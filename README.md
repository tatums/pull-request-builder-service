## pull-request-builder-service

## package
```bash
$ aws cloudformation package \
  --template-file resources.yaml \
  --output-template-file resources-spec.yaml \
  --s3-bucket pull-request-builder-service
```
## deploy
```bash
$ aws cloudformation deploy \
  --template-file resources-spec.yaml \
  --stack-name pull-request-builder-service \
  --capabilities CAPABILITY_IAM
```
