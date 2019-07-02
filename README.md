# sms-core
Cloudformation stack for send multiple SMS messages

## Exectution steps

1. Create Cloudfomtion stack by uploading template.yml

  - It will create following resources,
    - S3 Bucket (sms-sender-source-bucket) //Please change the bucket name in the template.yml, In 3 places
    - Lambda function (sms-sender-Lambda) //can be same
    - IAM Role (sms-sender-LambdaRole) //can be same

2. Upload data.csv file to the S3 bucket sms-sender-source-bucket


Be aware that SMS capability on AWS is limited to certain regions, make sure you refer https://docs.aws.amazon.com/sns/latest/dg/sms_supported-countries.html

   -Ideally create stack on us-east(Northern Virginia)
