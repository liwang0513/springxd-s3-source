# SPRINGXD-S3-Source
Features: 1) Can be scaled 2) Required Redis 3) Can only download to local disk

To use this module:

1) upload and register to XD module as Source
2) create a aws.properties file, the format is as sampleCredentials.properties inside this project
3) create the output folder in local disk
4) create and deploy the stream!

Example:

stream create test --definition "s3 --propertiesFile=/tmp/aws_amey.properties --bucket=liwang-test --containerNumber=1 --localDir=/tmp/out --redisHost=localhost | null" --deploy
