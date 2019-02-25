# GearSpotter.com landing page

## Infra

S3 bucket in CloudFormation stack. Install `awscli` first. To create the stack
for the first time:

    aws cloudformation create-stack --stack-name gs-landing --template-body file://$PWD/gs-landing.yaml
    
To update infra after changes to the stack:

    aws cloudformation update-stack --stack-name gs-landing --template-body file://$PWD/gs-landing.yaml

