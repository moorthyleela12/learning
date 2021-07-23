# learning notes

# to log into pcluster 

pcluster ssh -d cluster-leela10 -i ~/.aws/awsclusterictr.pem

ssh ubuntu@3.142.210.17 -i /Users/leelamoorthy/.aws/awsclusterictr.pem

# to copy script from directory to s3 
aws s3 cp /scratch/lmoorthy s3://parallelcluster-icdqe0cg8rq2ro1l/parallelcluster-cluster-leela10-3vx8ct5p0oetyx63 --recursive

# to see s3 bucket 
aws s3 ls

# to see specific bucket 
aws s3 ls s3://

# rename your s3 bucket name 
$ aws s3 mb s3://[new-bucket]
$ aws s3 sync s3://[old-bucket] s3://[new-bucket]
$ aws s3 rb --force s3://[old-bucket]
