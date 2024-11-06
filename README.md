# AWS CloudFormation - Creating stack
## Creating using existing template
1. navigate to aws CloudFormation console
2. Click on create stack and select use a sample template
3. Select a sample template from the dropdown and click next
4. Enter the neccessary details and click next
5. your stac should start creating and you can see the detail of your stack on the output

## Creating using custom template
There are 3 methods by which you can use custom template, here we are using sync from github option to auto deploy the changes to CloudFormation
1. fork this repo to your repo/clone and reupload this repo to your repo
2. on aws CloudFormation console, select create stack and select sync from git
3. link a git repo. here we are using github
4. select add a new connection
5. select github and click connect to git and allow access to specific repo that you want to sync
6. enter the specific .yaml/json filr path on git to sync
6. go to git and you will find a PR by CloudFormation. Accept the PR and rebase your repo
7. now changes done on the template that is specified will sync and deployed on respective resource

# Prerequisites
AWS Account: You need an AWS account to create resources.
EC2 Key Pair: You must have an existing EC2 Key Pair in the AWS region where you plan to deploy this stack. This key pair is used for SSH access to the instance.
AMI ID: The template uses a hardcoded AMI ID for Ubuntu 20.04. Make sure to replace it with the correct AMI ID for your region.
