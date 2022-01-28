# aws-cloudformation
A collection of CloudFormation templates to be used in StackSets for AWS organisation security and compliance.

## CloudFormation StackSets operation
CloudFormation StackSet have two modes of deployment, either with service-managed permissions or self-managed permissions. [StackSet concepts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-concepts.html)

Service-managed permissions means that CloudFormation is organisationally trusted and will be able
to deploy the required roles previous to deploying the resources declared in your CloudFormation StackSet template. It has a downside, which is that you can only target OUs within your organisation and not individual accounts.

Self-managed permissions require you to meet pre-requisites explained [StackSet prerequisites](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-prereqs.html), which can easily be completed using Terraform.

## CloudFormation StackSets templates
The examples in this repo are by no means a-perfect-usage examples, but working ones. Some of them are meant to be run in service-managed mode and some of them in self-managed mode, but it's not specified in each example.


