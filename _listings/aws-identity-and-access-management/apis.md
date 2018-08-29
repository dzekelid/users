---
name: AWS Identity and Access Management
x-slug: aws-identity-and-access-management
description: AWS Identity and Access Management (IAM) enables you to securely control
  access to AWS services and resources for your users. Using IAM, you can create and
  manage AWS users and groups, and use permissions to allow and deny their access
  to AWS resources.IAM is a feature of your AWS account offered at no additional charge.
  You will be charged only for use of other AWS services by your users.To get started
  using IAM, orif you have already registered with AWS, go to theAWS Management Consoleand
  get started with theseIAM Best Practices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Users
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Identity and Access Management API Create User
  x-api-slug: aws-identity-and-access-management-api
  description: Creates a new IAM user for your AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=CreateUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/actioncreateuser-get-openapi.md
- name: AWS Identity and Access Management API Delete User
  x-api-slug: aws-identity-and-access-management-api
  description: Deletes the specified IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=DeleteUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/actiondeleteuser-get-openapi.md
- name: AWS Identity and Access Management API Get User
  x-api-slug: aws-identity-and-access-management-api
  description: |-
    Retrieves information about the specified IAM user, including the user's creation
          date, path, unique ID, and ARN.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=GetUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/actiongetuser-get-openapi.md
- name: AWS Identity and Access Management API List Users
  x-api-slug: aws-identity-and-access-management-api
  description: Lists the IAM users that have the specified path prefix.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListUsers
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/actionlistusers-get-openapi.md
- name: AWS Identity and Access Management API Put User Policy
  x-api-slug: aws-identity-and-access-management-api
  description: |-
    Adds or updates an inline policy document that is embedded in the specified IAM
          user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=PutUserPolicy
  tags: Users Policies
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/actionputuserpolicy-get-openapi.md
- name: AWS Identity and Access Management API Update User
  x-api-slug: aws-identity-and-access-management-api
  description: Updates the name and/or the path of the specified IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=UpdateUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/actionupdateuser-get-openapi.md
- name: AWS Identity and Access Management API
  x-api-slug: aws-identity-and-access-management-api
  description: AWS Identity and Access Management (IAM) enables you to securely control
    access to AWS services and resources for your users. Using IAM, you can create
    and manage AWS users and groups, and use permissions to allow and deny their access
    to AWS resources.IAM is a feature of your AWS account offered at no additional
    charge. You will be charged only for use of other AWS services by your users.To
    get started using IAM, orif you have already registered with AWS, go to theAWS
    Management Consoleand get started with theseIAM Best Practices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-identity-and-access-management/openapi.md
x-common:
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=323
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sts/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/IAM/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/iam/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=76
- type: x-getting-started
  url: https://aws.amazon.com/iam/getting-started/
- type: x-partners
  url: https://aws.amazon.com/iam/partners/
- type: x-tools
  url: http://aws.amazon.com/cli
- type: x-website
  url: https://aws.amazon.com/iam/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---