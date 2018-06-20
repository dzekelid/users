---
name: AWS WorkDocs
x-slug: aws-workdocs
description: Amazon WorkDocs is a fully managed, secure enterprise storage and sharing
  service with strong administrative controls and feedback capabilities that improve
  user productivity.Users can comment on files, send them to others for feedback,
  and upload new versions without having to resort to emailing multiple versions of
  their files as attachments. Users can take advantage of these capabilities wherever
  they are, using the device of their choice, including PCs, Macs, tablets and phones.
  Amazon WorkDocs offers IT administrators the option of integrating with existing
  corporate directories, flexible sharing policies and control of the location where
  data is stored. Customers can get started using Amazon WorkDocs with a 30-day free
  trial providing 1 TB of storage per user for up to 50 users.Amazon WorkDocs offers
  an Administrative SDK, currently in public preview. The Administrative SDK allows
  you to integrate your applications with Amazon WorkDocs by performing content and
  permissions updates, and managing users, programmatically. You can sign-up for the
  public preview here.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/apis.md
specificationVersion: "0.14"
apis:
- name: AWS WorkDocs API Activate User
  x-api-slug: aws-workdocs-api
  description: Activates the specified user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: ://///?Action=ActivateUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/actionactivateuser-get-openapi.md
- name: AWS WorkDocs API Create User
  x-api-slug: aws-workdocs-api
  description: Creates a user in a Simple AD or Microsoft AD directory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: ://///?Action=CreateUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/actioncreateuser-get-openapi.md
- name: AWS WorkDocs API Deactivate User
  x-api-slug: aws-workdocs-api
  description: Deactivates the specified user, which revokes the user's access to
    Amazon WorkDocs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: ://///?Action=DeactivateUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/actiondeactivateuser-get-openapi.md
- name: AWS WorkDocs API Delete User
  x-api-slug: aws-workdocs-api
  description: Deletes the specified user from a Simple AD or Microsoft AD directory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: ://///?Action=DeleteUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/actiondeleteuser-get-openapi.md
- name: AWS WorkDocs API Describe Users
  x-api-slug: aws-workdocs-api
  description: Describes the specified users.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: ://///?Action=DescribeUsers
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/actiondescribeusers-get-openapi.md
- name: AWS WorkDocs API Update User
  x-api-slug: aws-workdocs-api
  description: "Updates the specified attributes of the specified user, and grants
    or revokes \n      administrative privileges to the Amazon WorkDocs site."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: ://///?Action=UpdateUser
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/actionupdateuser-get-openapi.md
- name: AWS WorkDocs API
  x-api-slug: aws-workdocs-api
  description: Amazon WorkDocs is a fully managed, secure enterprise storage and sharing
    service with strong administrative controls and feedback capabilities that improve
    user productivity.Users can comment on files, send them to others for feedback,
    and upload new versions without having to resort to emailing multiple versions
    of their files as attachments. Users can take advantage of these capabilities
    wherever they are, using the device of their choice, including PCs, Macs, tablets
    and phones. Amazon WorkDocs offers IT administrators the option of integrating
    with existing corporate directories, flexible sharing policies and control of
    the location where data is stored. Customers can get started using Amazon WorkDocs
    with a 30-day free trial providing 1 TB of storage per user for up to 50 users.Amazon
    WorkDocs offers an Administrative SDK, currently in public preview. The Administrative
    SDK allows you to integrate your applications with Amazon WorkDocs by performing
    content and permissions updates, and managing users, programmatically. You can
    sign-up for the public preview here.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Enterprise-Applications_AmazonWorkDocs.png
  humanURL: https://aws.amazon.com/workdocs/
  baseURL: :///
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-workdocs/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/workdocs/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/workdocs/faqs/
- type: x-forum
  url: https://aws.amazon.com/workdocs/resources/#forum
- type: x-pricing
  url: https://aws.amazon.com/workdocs/pricing/
- type: x-sdk
  url: https://aws.amazon.com/workdocs/developers/
- type: x-website
  url: https://aws.amazon.com/workdocs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---