# Release Process

This document describes how to create a new release of the Rundeck Go SDK.

## Automated Releases

Releases are automated via GitHub Actions. When you push a version tag, a release is automatically created.

## Creating a Release

### 1. Prepare the Release

Ensure all changes are merged to `master`:

```bash
git checkout master
git pull origin master
```

### 2. Choose Version Number

Follow [Semantic Versioning](https://semver.org/):

- **MAJOR** version (v2.0.0): Incompatible API changes
- **MINOR** version (v1.1.0): New functionality, backwards compatible
- **PATCH** version (v1.0.1): Bug fixes, backwards compatible

### 3. Create and Push Tag

```bash
# Create an annotated tag
git tag -a v1.0.0 -m "Release v1.0.0"

# Push the tag to GitHub
git push origin v1.0.0
```

### 4. Monitor Release

The GitHub Actions workflow will:
1. ✅ Run tests
2. ✅ Build the SDK
3. ✅ Generate changelog
4. ✅ Create GitHub release
5. ✅ Notify Go proxy

Check the [Actions tab](https://github.com/rundeck/go-rundeck/actions) to monitor progress.

### 5. Verify Release

Once complete, verify the release:

```bash
# Check Go proxy has the version
curl https://proxy.golang.org/github.com/rundeck/go-rundeck/rundeck-v2/@v/v1.0.0.info

# Test installation
go get github.com/rundeck/go-rundeck/rundeck-v2@v1.0.0
```

## Using the Released Version

### In go.mod

```go
require (
    github.com/rundeck/go-rundeck/rundeck-v2 v1.0.0
)
```

### In your code

```bash
go get github.com/rundeck/go-rundeck/rundeck-v2@v1.0.0
```

## Pre-release Versions

For testing before official release:

```bash
# Create pre-release tag
git tag -a v1.0.0-rc.1 -m "Release Candidate 1"
git push origin v1.0.0-rc.1
```

Pre-release tags (with `-rc`, `-beta`, `-alpha` suffixes) will be marked as pre-releases on GitHub.

## Troubleshooting

### Release Failed

If the GitHub Action fails:
1. Check the [Actions logs](https://github.com/rundeck/go-rundeck/actions)
2. Fix the issue
3. Delete the tag locally and remotely:
   ```bash
   git tag -d v1.0.0
   git push origin :refs/tags/v1.0.0
   ```
4. Create and push the tag again

### Go Proxy Not Updated

The Go proxy can take a few minutes to index new versions:

```bash
# Manually trigger proxy update
curl "https://proxy.golang.org/github.com/rundeck/go-rundeck/rundeck-v2/@v/v1.0.0.info"
```

### Version Conflicts

If you need to replace a version:
1. Delete the GitHub release
2. Delete the tag (locally and remotely)
3. Recreate with the same version
4. Note: Go proxy caches are immutable, so consumers may need to clear their cache

## Release Checklist

Before creating a release:

- [ ] All tests pass
- [ ] SDK compiles without errors
- [ ] OpenAPI spec is valid
- [ ] README is up to date
- [ ] Breaking changes are documented
- [ ] Version number follows semver
- [ ] CHANGELOG entries are meaningful

## Future Enhancements

Potential improvements to the release process:

1. **Automated changelog**: Use conventional commits
2. **Release notes template**: Pre-fill with PR titles
3. **Version bumping script**: Auto-increment versions
4. **Integration tests**: Test against live Rundeck instance
5. **API compatibility checks**: Detect breaking changes

## Questions?

Open an issue or discussion on GitHub.

