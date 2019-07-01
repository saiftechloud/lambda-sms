# sms-core
Cloudformation stack for send multiple SMS messages

## Exectution steps

1. Create Cloudfomtion stack by uploading template.yml

  - It will create following resources,
    - S3 Bucket (sms-sender-source-bucket)
    - Lambda function (sms-sender-Lambda)
    - IAM Role (sms-sender-LambdaRole)

2. Upload data.csv file to the S3 bucket sms-sender-source-bucket
