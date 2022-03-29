# Project2

Run the files in order:

Run network file:

aws cloudformation create-stack --stack-name udagram-network --template-body file://final-code-network.yml --parameters file://network-parameters.json --region=us-east-1 --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" --no-verify-ssl

Once complete, run server file: aws cloudformation create-stack --stack-name udagram-server --template-body file://final-code-servers.yml --parameters file://server-parameters.json --region=us-east-1 --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" --no-verify-ssl
