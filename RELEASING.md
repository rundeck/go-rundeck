# Release Process

This document describes how to create a new release of the Rundeck Go SDK.

## Multi-Module Repository

This repository contains **two independent Go modules**:

- **`rundeck-v2/`** - Modern SDK (OpenAPI Generator, API v56) ⭐ **Recommended**
- **`rundeck/`** - Legacy SDK (AutoRest-based) ⚠️ **Deprecated**

Each module is versioned independently using **module-prefixed tags**.

---

## Quick Start

### Release rundeck-v2 (Most Common)

```bash
# 1. Ensure you're on master with latest changes
git checkout master
git pull origin master

# 2. Create and push module-prefixed tag
git tag -a rundeck-v2/v1.3.0 -m "Release rundeck-v2 v1.3.0"
git push origin rundeck-v2/v1.3.0

# 3. Done! GitHub Actions automatically:
#    ✅ Builds the SDK
#    ✅ Runs tests
#    ✅ Creates release with notes
#    ✅ Updates Go proxy
```

---

## Tag Formats

### Module-Prefixed Tags (Required for Go Modules)

Go's module system requires tags to be prefixed with the module path:

| Tag Format | Module | Use Case |
|------------|--------|----------|
| `rundeck-v2/v1.3.0` | rundeck-v2 | **Use this** for v2 SDK releases |
| `rundeck/v1.3.0` | rundeck | Legacy SDK (rarely needed) |
| `v1.3.0` | Both | Combined release (avoid unless intentional) |

**Why?** In multi-module repos, Go needs the prefix to know which module you're releasing.

---

## Creating a Release

### 1. Prepare the Release

Ensure all changes are merged to `master`:

```bash
git checkout master
git pull origin master
```

### 2. Choose Version Number

Follow [Semantic Versioning](https://semver.org/):

- **MAJOR** (v2.0.0): Breaking API changes
- **MINOR** (v1.1.0): New features, backwards compatible
- **PATCH** (v1.0.1): Bug fixes, backwards compatible

**Note:** `rundeck-v2` and `rundeck` versions are independent. They don't need to match.

### 3. Create Module-Prefixed Tag

**For rundeck-v2 (recommended):**

```bash
git tag -a rundeck-v2/v1.3.0 -m "Release rundeck-v2 v1.3.0

- Add new feature X
- Fix bug Y
- Update to API v56"

git push origin rundeck-v2/v1.3.0
```

**For rundeck (legacy, rare):**

```bash
git tag -a rundeck/v1.3.0 -m "Release rundeck v1.3.0"
git push origin rundeck/v1.3.0
```

### 4. Monitor Release

GitHub Actions will automatically:

1. ✅ Detect the module from the tag
2. ✅ Build the specific module
3. ✅ Run tests
4. ✅ Generate changelog since last module release
5. ✅ Create GitHub release with module-specific notes
6. ✅ Update Go proxy

**Watch progress:** [GitHub Actions](https://github.com/rundeck/go-rundeck/actions)

### 5. Verify Release

Once complete, verify the release:

```bash
# Check Go proxy has the version (wait 1-2 minutes)
curl https://proxy.golang.org/github.com/rundeck/go-rundeck/rundeck-v2/@v/v1.3.0.info

# Test installation
mkdir /tmp/test-sdk && cd /tmp/test-sdk
go mod init test
go get github.com/rundeck/go-rundeck/rundeck-v2@v1.3.0
```

---

## Using Released Versions

### In go.mod

**rundeck-v2 (recommended):**
```go
require (
    github.com/rundeck/go-rundeck/rundeck-v2 v1.3.0
)
```

**rundeck (legacy):**
```go
require (
    github.com/rundeck/go-rundeck/rundeck v1.3.0
)
```

### Install via CLI

```bash
# Install rundeck-v2
go get github.com/rundeck/go-rundeck/rundeck-v2@v1.3.0

# Or rundeck (legacy)
go get github.com/rundeck/go-rundeck/rundeck@v1.3.0
```

---

## Pre-release Versions

For testing before official release:

```bash
# Create pre-release tag
git tag -a rundeck-v2/v1.3.0-rc.1 -m "Release Candidate 1"
git push origin rundeck-v2/v1.3.0-rc.1
```

Pre-release suffixes: `-rc`, `-beta`, `-alpha`

These are automatically marked as pre-releases on GitHub.

---

## Release Notes

The workflow automatically generates module-specific release notes:

### rundeck-v2 Release Notes Include:
- ✨ Feature highlights (196 endpoints, Runner API, etc.)
- 📦 Installation instructions
- 📝 Changelog since last v2 release
- 📚 Documentation links
- 🔧 Go compatibility info

### rundeck Release Notes Include:
- ⚠️ Deprecation warning
- 🔄 Migration guide to rundeck-v2
- 📦 Installation instructions
- 📝 Changelog since last legacy release

---

## Troubleshooting

### Release Workflow Failed

If the GitHub Action fails:

1. **Check the logs:**
   - Go to [Actions tab](https://github.com/rundeck/go-rundeck/actions)
   - Click the failed workflow run
   - Review error messages

2. **Fix the issue** (common causes):
   - Build errors in SDK
   - Test failures
   - Invalid tag format

3. **Delete and recreate the tag:**
   ```bash
   # Delete locally
   git tag -d rundeck-v2/v1.3.0
   
   # Delete remotely
   git push origin :refs/tags/rundeck-v2/v1.3.0
   
   # Fix the issue, then recreate
   git tag -a rundeck-v2/v1.3.0 -m "Release rundeck-v2 v1.3.0"
   git push origin rundeck-v2/v1.3.0
   ```

### Go Proxy Not Updated

The Go proxy can take 1-5 minutes to index new versions:

```bash
# Manually trigger proxy update
curl "https://proxy.golang.org/github.com/rundeck/go-rundeck/rundeck-v2/@v/v1.3.0.info"

# Check if it's available
curl "https://sum.golang.org/lookup/github.com/rundeck/go-rundeck/rundeck-v2@v1.3.0"
```

If it still doesn't appear after 10 minutes:
- Verify the tag exists: `git ls-remote --tags origin`
- Check that `go.mod` has correct module path
- Ensure the release workflow completed successfully

### Wrong Module Released

If you tagged the wrong module:

1. Delete the release on GitHub
2. Delete the tag:
   ```bash
   git tag -d rundeck-v2/v1.3.0
   git push origin :refs/tags/rundeck-v2/v1.3.0
   ```
3. Create the correct tag

**Note:** Go proxy caches are immutable. If the wrong version was published, you'll need to bump to the next version.

### Tag Without Module Prefix

If you accidentally created a root tag (e.g., `v1.3.0`):

1. This creates a **combined release** for both modules
2. Usually not what you want
3. Delete and recreate with module prefix

---

## Release Checklist

Before creating a release:

- [ ] All changes merged to `master`
- [ ] Tests pass locally: `cd rundeck-v2 && go test ./...`
- [ ] SDK builds: `cd rundeck-v2 && go build`
- [ ] OpenAPI spec is valid
- [ ] README is up to date
- [ ] Breaking changes are documented (for MAJOR versions)
- [ ] Version number follows semver
- [ ] Using correct tag format: `rundeck-v2/v*.*.*`

---

## Version History Best Practices

### Independent Versioning

Each module maintains its own version history:

```
rundeck-v2/v1.0.0  → First release of v2
rundeck-v2/v1.1.0  → Add new features to v2
rundeck-v2/v1.2.0  → More v2 features

rundeck/v1.0.0     → Legacy SDK release (independent)
```

### When to Increment

**rundeck-v2:**
- **MAJOR:** Breaking changes to v2 API
- **MINOR:** New endpoints, new features
- **PATCH:** Bug fixes, documentation

**rundeck (legacy):**
- Only release if critical security/bug fixes needed
- Otherwise, direct users to rundeck-v2

### Recommended Strategy

For new development:
1. ✅ Release `rundeck-v2/vX.Y.Z` regularly
2. ⚠️ Avoid releasing `rundeck/vX.Y.Z` (deprecated)
3. ❌ Avoid root tags `vX.Y.Z` (ambiguous)

---

## Examples

### Example 1: New Feature Release

```bash
# Scenario: Added job tags query endpoints to rundeck-v2
git checkout master
git pull origin master

# Current version is v1.2.0, adding features → v1.3.0 (MINOR bump)
git tag -a rundeck-v2/v1.3.0 -m "Release rundeck-v2 v1.3.0

Features:
- Add job tags query endpoints
- Improve error handling
- Update to API v56"

git push origin rundeck-v2/v1.3.0
```

### Example 2: Bug Fix Release

```bash
# Scenario: Fixed error response parsing bug
git checkout master
git pull origin master

# Current version is v1.3.0, bug fix → v1.3.1 (PATCH bump)
git tag -a rundeck-v2/v1.3.1 -m "Release rundeck-v2 v1.3.1

Fixes:
- Fix ApiErrorResponse boolean parsing
- Correct enum value cases"

git push origin rundeck-v2/v1.3.1
```

### Example 3: Breaking Change Release

```bash
# Scenario: Changed SDK architecture (rare)
git checkout master
git pull origin master

# Current version is v1.9.0, breaking changes → v2.0.0 (MAJOR bump)
git tag -a rundeck-v2/v2.0.0 -m "Release rundeck-v2 v2.0.0

BREAKING CHANGES:
- Restructured client initialization
- Renamed methods for consistency
- Updated error handling

See MIGRATION.md for upgrade guide"

git push origin rundeck-v2/v2.0.0
```

---

## Advanced: Combined Releases

To release both modules with the same version (rare):

```bash
# This creates a single release for both modules
git tag -a v2.0.0 -m "Release v2.0.0"
git push origin v2.0.0
```

**When to use:**
- Major milestones affecting both modules
- Synchronized version numbers for simplicity

**Usually better to:**
- Use module-specific tags for clarity

---

## Questions?

- **Issues:** [GitHub Issues](https://github.com/rundeck/go-rundeck/issues)
- **Discussions:** [GitHub Discussions](https://github.com/rundeck/go-rundeck/discussions)
- **Rundeck Docs:** [docs.rundeck.com](https://docs.rundeck.com)

---

## Additional Resources

- [Go Modules Multi-Module Repos](https://go.dev/wiki/Modules#faqs--multi-module-repositories)
- [Semantic Versioning](https://semver.org/)
- [GitHub Releases](https://docs.github.com/en/repositories/releasing-projects-on-github)
- [Go Module Proxy](https://proxy.golang.org/)
