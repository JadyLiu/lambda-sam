Lambda SAM deployment command:

```
sudo pip install awscli
aws cloudformation package --template-file app-spec.yml --output-template-file app-spec.deploy --s3-bucket $S3_BUCKET_NAME
aws cloudformation deploy --template-file app-spec.deploy --stack-name $STACK_NAME --capabilities CAPABILITY_IAM
```
