---
title: 02d - Cloud Formation
tags:
  - aws
---

Cloud Formation is an *Infrastructure as Code (IaC)* product in AWS which allows automation infrastructure creation, update and deletion using templates.

Templates created in YAML or JSON can be used to automate infrastructure operations.
Templates are used to create stacks, which are used to interact with resources in an AWS account.

All templates will have a list of resources, this is the only required section of a template, because without it a template would be useless.

**NOTE**: A trick question that gets asked is if you use the `AWSTemplateFormatVersion` + `description` you must ensure that you have description right have the version. This is required in that specific scenario.

## Template Fields

**AWSTemplateFormatVersion** - AWS Version of template
**Description** - Describes template to a user
**Metadata** - 
**Parameters** - Can add fields to prompt user for more information
**Mappings** - Allows you to create lookup tables
**Conditions** - These things will only occur when conditions are met. So if a param or something meets a set condition.
**Transform** - 
**Resources** - 
**Outputs** - Outputs from the template being applied. This could be almost anything.

### How it works?

Resources inside of a template are called *Logical Resources*, and example would be a template that has a resource for and EC2 instance.

When you take a template and give it to Cloud Formation, it then goes and creates what's called a *stack* and this contains all the resources, it is the living representation of the template.

For any logical resources in the stack, it will then create the actual physical resource, so a real EC2 instance.

![[Pasted image 20230901144233.png]]

## Creating a stack

1) Head to Cloud Formation on the dashboard and click create a stack
2) Use a template, create, or pick from a sample. Example: [[@Basic EC2 Template]]
3) Fill in remaining options
4) Create new stack