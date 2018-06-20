---
name: AWS Cognito
x-slug: aws-cognito
description: Amazon Cognito lets you easily add user sign-up and sign-in to your mobile
  and web apps. With Amazon Cognito, you also have the options to authenticate users
  through social identity providers such as Facebook, Twitter, or Amazon, with SAML
  identity solutions, or by using your own identity system. In addition, Amazon Cognito
  enables you to save data locally on users devices, allowing your applications to
  work even when the devices are offline. You can then synchronize data across users
  devices so that their app experience remains consistent regardless of the device
  they use. With Amazon Cognito, you can focus on creating great app experiences instead
  of worrying about building, securing, and scaling a solution to handle user management,
  authentication, and sync across devices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Users
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Cognito API Admin Add User To Group
  x-api-slug: aws-cognito-api
  description: Adds the specified user to the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminAddUserToGroup
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminaddusertogroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminaddusertogroup-get-openapi.md
- name: AWS Cognito API Admin Create User
  x-api-slug: aws-cognito-api
  description: |-
    Creates a new user in the specified user pool and sends a welcome message via email
                or phone (SMS).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminCreateUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmincreateuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmincreateuser-get-openapi.md
- name: AWS Cognito API Admin Delete User
  x-api-slug: aws-cognito-api
  description: Deletes a user as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminDeleteUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmindeleteuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmindeleteuser-get-openapi.md
- name: AWS Cognito API Admin Delete User Attributes
  x-api-slug: aws-cognito-api
  description: Deletes the user attributes in a user pool as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminDeleteUserAttributes
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmindeleteuserattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmindeleteuserattributes-get-openapi.md
- name: AWS Cognito API Admin Disable User
  x-api-slug: aws-cognito-api
  description: Disables the specified user as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminDisableUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmindisableuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmindisableuser-get-openapi.md
- name: AWS Cognito API Admin Enable User
  x-api-slug: aws-cognito-api
  description: Enables the specified user as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminEnableUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminenableuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminenableuser-get-openapi.md
- name: AWS Cognito API Admin Get User
  x-api-slug: aws-cognito-api
  description: Gets the specified user by user name in a user pool as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminGetUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmingetuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadmingetuser-get-openapi.md
- name: AWS Cognito API Admin List Groups For User
  x-api-slug: aws-cognito-api
  description: Lists the groups that the user belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminListGroupsForUser
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminlistgroupsforuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminlistgroupsforuser-get-openapi.md
- name: AWS Cognito API Admin Remove User From Group
  x-api-slug: aws-cognito-api
  description: Removes the specified user from the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminRemoveUserFromGroup
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminremoveuserfromgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminremoveuserfromgroup-get-openapi.md
- name: AWS Cognito API Admin Reset User Password
  x-api-slug: aws-cognito-api
  description: Resets the specified user's password in a user pool as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminResetUserPassword
  tags: Users,Passwords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminresetuserpassword-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminresetuserpassword-get-openapi.md
- name: AWS Cognito API Admin Set User Settings
  x-api-slug: aws-cognito-api
  description: Sets all the user settings for a specified user name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminSetUserSettings
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminsetusersettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminsetusersettings-get-openapi.md
- name: AWS Cognito API Admin Update Device Status
  x-api-slug: aws-cognito-api
  description: Updates the device status as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminUpdateDeviceStatus
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminupdatedevicestatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminupdatedevicestatus-get-openapi.md
- name: AWS Cognito API Admin Update User Attributes
  x-api-slug: aws-cognito-api
  description: |-
    Updates the specified user's attributes, including developer attributes, as an
                administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminUpdateUserAttributes
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminupdateuserattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminupdateuserattributes-get-openapi.md
- name: AWS Cognito API Admin User Global Sign Out
  x-api-slug: aws-cognito-api
  description: Signs out users from all devices, as an administrator.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminUserGlobalSignOut
  tags: Users,Global Sign Out
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminuserglobalsignout-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionadminuserglobalsignout-get-openapi.md
- name: AWS Cognito API Create User Import Job
  x-api-slug: aws-cognito-api
  description: Creates the user import job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=CreateUserImportJob
  tags: Users,Imports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actioncreateuserimportjob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actioncreateuserimportjob-get-openapi.md
- name: AWS Cognito API Create User Pool
  x-api-slug: aws-cognito-api
  description: |-
    Creates a new Amazon Cognito user pool and sets the password policy for the
                pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=CreateUserPool
  tags: Users,Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actioncreateuserpool-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actioncreateuserpool-get-openapi.md
- name: AWS Cognito API Create User Pool Client
  x-api-slug: aws-cognito-api
  description: Creates the user pool client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=CreateUserPoolClient
  tags: Users,Pool Clients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actioncreateuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actioncreateuserpoolclient-get-openapi.md
- name: AWS Cognito API Delete User
  x-api-slug: aws-cognito-api
  description: Allows a user to delete one's self.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DeleteUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuser-get-openapi.md
- name: AWS Cognito API Delete User Attributes
  x-api-slug: aws-cognito-api
  description: Deletes the attributes for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DeleteUserAttributes
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuserattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuserattributes-get-openapi.md
- name: AWS Cognito API Delete User Pool
  x-api-slug: aws-cognito-api
  description: Deletes the specified Amazon Cognito user pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DeleteUserPool
  tags: Users,Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuserpool-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuserpool-get-openapi.md
- name: AWS Cognito API Delete User Pool Client
  x-api-slug: aws-cognito-api
  description: Allows the developer to delete the user pool client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DeleteUserPoolClient
  tags: Users,Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondeleteuserpoolclient-get-openapi.md
- name: AWS Cognito API Describe User Import Job
  x-api-slug: aws-cognito-api
  description: Describes the user import job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DescribeUserImportJob
  tags: Users,Imports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondescribeuserimportjob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondescribeuserimportjob-get-openapi.md
- name: AWS Cognito API Describe User Pool
  x-api-slug: aws-cognito-api
  description: |-
    Returns the configuration information and metadata of the specified user
                pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DescribeUserPool
  tags: Users,Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondescribeuserpool-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondescribeuserpool-get-openapi.md
- name: AWS Cognito API Describe User Pool Client
  x-api-slug: aws-cognito-api
  description: |-
    Client method for returning the configuration information and metadata of the
                specified user pool client.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DescribeUserPoolClient
  tags: Users,Pool Clients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondescribeuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiondescribeuserpoolclient-get-openapi.md
- name: AWS Cognito API Get Device
  x-api-slug: aws-cognito-api
  description: Gets the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=GetDevice
  tags: Users,Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiongetdevice-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiongetdevice-get-openapi.md
- name: AWS Cognito API Get User
  x-api-slug: aws-cognito-api
  description: Gets the user attributes and metadata for a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=GetUser
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiongetuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actiongetuser-get-openapi.md
- name: AWS Cognito API List User Import Jobs
  x-api-slug: aws-cognito-api
  description: Lists the user import jobs.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ListUserImportJobs
  tags: Users,Imports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionlistuserimportjobs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionlistuserimportjobs-get-openapi.md
- name: AWS Cognito API List Users
  x-api-slug: aws-cognito-api
  description: Lists the users in the Amazon Cognito user pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ListUsers
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionlistusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionlistusers-get-openapi.md
- name: AWS Cognito API List Users In Group
  x-api-slug: aws-cognito-api
  description: Lists the users in the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ListUsersInGroup
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionlistusersingroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionlistusersingroup-get-openapi.md
- name: AWS Cognito API Set User Settings
  x-api-slug: aws-cognito-api
  description: Sets the user settings like multi-factor authentication (MFA).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=SetUserSettings
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionsetusersettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionsetusersettings-get-openapi.md
- name: AWS Cognito API Start User Import Job
  x-api-slug: aws-cognito-api
  description: Starts the user import.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=StartUserImportJob
  tags: Users,Imports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionstartuserimportjob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionstartuserimportjob-get-openapi.md
- name: AWS Cognito API Stop User Import Job
  x-api-slug: aws-cognito-api
  description: Stops the user import job.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=StopUserImportJob
  tags: Users,Iimport
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionstopuserimportjob-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionstopuserimportjob-get-openapi.md
- name: AWS Cognito API Update User Attributes
  x-api-slug: aws-cognito-api
  description: Allows a user to update a specific attribute (one at a time).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=UpdateUserAttributes
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionupdateuserattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionupdateuserattributes-get-openapi.md
- name: AWS Cognito API Update User Pool
  x-api-slug: aws-cognito-api
  description: Updates the specified user pool with the specified attributes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=UpdateUserPool
  tags: Users,Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionupdateuserpool-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionupdateuserpool-get-openapi.md
- name: AWS Cognito API Update User Pool Client
  x-api-slug: aws-cognito-api
  description: |-
    Allows the developer to update the specified user pool client and password
                policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=UpdateUserPoolClient
  tags: Users,Pool Clients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionupdateuserpoolclient-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionupdateuserpoolclient-get-openapi.md
- name: AWS Cognito API Verify User Attribute
  x-api-slug: aws-cognito-api
  description: Verifies the specified user attributes in the user pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=VerifyUserAttribute
  tags: Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionverifyuserattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/actionverifyuserattribute-get-openapi.md
- name: AWS Cognito API
  x-api-slug: aws-cognito-api
  description: Amazon Cognito lets you easily add user sign-up and sign-in to your
    mobile and web apps. With Amazon Cognito, you also have the options to authenticate
    users through social identity providers such as Facebook, Twitter, or Amazon,
    with SAML identity solutions, or by using your own identity system. In addition,
    Amazon Cognito enables you to save data locally on users devices, allowing your
    applications to work even when the devices are offline. You can then synchronize
    data across users devices so that their app experience remains consistent regardless
    of the device they use. With Amazon Cognito, you can focus on creating great app
    experiences instead of worrying about building, securing, and scaling a solution
    to handle user management, authentication, and sync across devices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/users/master/_listings/aws-cognito/openapi.md
x-common:
- type: x-blog
  url: https://aws.amazon.com/cognito/dev-resources/#blogposts
- type: x-documentation
  url: http://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitoidentity/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitosync/latest/APIReference/Welcome.html
- type: x-faq
  url: http://aws.amazon.com/cognito/faqs
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=173
- type: x-pricing
  url: http://aws.amazon.com/cognito/pricing
- type: x-sdk
  url: https://aws.amazon.com/cognito/dev-resources/#documentation
- type: x-slides
  url: https://aws.amazon.com/cognito/dev-resources/#slides
- type: x-videos
  url: https://aws.amazon.com/cognito/dev-resources/#videos
- type: x-website
  url: https://aws.amazon.com/cognito/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---