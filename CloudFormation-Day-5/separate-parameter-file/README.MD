### The command below creates a Cloud Formation stack using a separate parameter file
aws cloudformation create-stack --stack-name dev-network-infra-pf --template-body file://network-infra.yaml --parameters file://dev-parameter-file.json

### The command below deletes the stack from Cloud Formation
aws cloudformation delete-stack --stack-name dev-network-infra-pf

aws cloudformation update-stack --stack-name dev-network-infra-pf --template-body file://network-infra.yaml --parameters file://dev-parameter-file.json