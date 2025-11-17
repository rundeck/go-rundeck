
# Rundeck Go Client V2

```bash
openapi-generator generate \
  -i rundeck-api.yml \
  -g go \
  --git-user-id rundeck \
  --git-repo-id go-rundeck/rundeck-v2 \
  -o ./rundeck-v2 
```

```bash
cd rundeck-v2
go mod tidy
go mod vendor   
go install
```