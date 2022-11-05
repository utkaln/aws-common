### Useful CLI Commands

#### check user details from CLI
> aws sts get-caller-identity


#### upload a local file to S3
> aws s3 cp /Users/utkalnayak/Documents/aws/test-data s3://s3-learn-utkal --recursive


#### remove a file from s3 bucket
> aws s3 rm s3://trvpiij22/house1.jpeg --recursive

#### copy local file to s3
> aws s3 cp house1.jpeg s3://trvpiij22


### CLEAN UP

#### list lambda with date filter
> aws lambda list-functions --query 'Functions[?LastModified > `` `2022-09-01` ``].[FunctionName,LastModified]'

#### delete lambda
> aws lambda delete-function --function-name my-function



