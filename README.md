# CloudFormation

It might be challenging to manage an infrastructure with numerous services. Multiple AWS resource creation and management can be difficult and time-consuming. In fact, if you do those things, you can find yourself spending a lot of time managing your AWS resources rather than creating new applications. How can we fix this issue?

An aid is AWS CloudFormation. As previously mentioned, it gives you a straightforward method for building and managing a group of AWS resources by provisioning and updating them in a systematic and predictable way. Simply put, it enables you to model and build your infrastructure and applications without having to carry out manual processes. You can manage all of your infrastructure and AWS resources in a text file or template using AWS CloudFormation. A stack is a grouping of AWS resources. A stack can be used to create or modify AWS resources.

Using templates, you may quickly deploy all the resources your application needs. Additionally, you can replicate your infrastructure using your templates across several settings. Use the templates' parameters, mappings, and conditions sections to make them reusable and allow you to personalise your stack creations.

- Using the JSON or YAML formats, make a new template or use an existing CloudFormation template.
- Locally or in an S3 bucket, save your code template.
- Create a stack based on your template using AWS CloudFormation.
- Your template's specified stack resources are built and configured by AWS CloudFormation.

## Problems

- There is very high cost to maintain the servers with storages, Congiguration and dependencies.
- Extra cost for Backup with AMI, generally for storage
- Manually setup of the whole infrasture is time consuming and inefficient.
- There are chances of error due to manual process.

## Solution

- CloudFormation is an ideal tool to Automate the AWS Stack.
- Automatic Setup of the whole infrastrure with any human erorrs due to manual process.
- Maintain state if each and every Infrastruture.
- All the dependies with their Version Control service.
- Repeatable and reusable.

### Templates:

1. It's a Text file which can be YAML or JSON.
2. These files serves as input template for the CloudFormation.
3. These templates descries the state of Infrastructure.
4. THese templates are first read by CloudFormation to create the stack.
5. Templates can be updated to make changes.
6. These Resources are putted together as a single unit.

### Change Set:

1. Before Updating a stack, you have a choice to generate a change set.
2. A change set allows you to see how chanes will impact your existing resources, so that you have chance to save your data or to make backup.
3. When working with live systems:
   - It will create a new intance when change is intiated
   - It will delete the old stack, which can result in Data Loss.
