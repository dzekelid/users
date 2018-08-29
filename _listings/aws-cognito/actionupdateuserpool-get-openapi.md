---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Update User Pool
  version: 1.0.0
  description: Updates the specified user pool with the specified attributes.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminAddUserToGroup:
    get:
      summary: Admin Add User To Group
      description: Adds the specified user to the specified group.
      operationId: adminAddUserToGroup
      x-api-path-slug: actionadminaddusertogroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminCreateUser:
    get:
      summary: Admin Create User
      description: |-
        Creates a new user in the specified user pool and sends a welcome message via email
                    or phone (SMS).
      operationId: adminCreateUser
      x-api-path-slug: actionadmincreateuser-get
      parameters:
      - in: query
        name: DesiredDeliveryMediums
        description: Specify EMAIL if email will be used to send the welcome message
        type: string
      - in: query
        name: ForceAliasCreation
        description: This parameter is only used if the phone_number_verified or email_verified            attribute
          is set to True
        type: string
      - in: query
        name: MessageAction
        description: Set to RESEND to resend the invitation message to a user that
          already exists and            reset the expiration limit on the users account
        type: string
      - in: query
        name: TemporaryPassword
        description: The users temporary password
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs that contain user attributes and
          attribute values to            be set for the user to be created
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where the user will be created
        type: string
      - in: query
        name: ValidationData
        description: The users validation data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDeleteUser:
    get:
      summary: Admin Delete User
      description: Deletes a user as an administrator.
      operationId: adminDeleteUser
      x-api-path-slug: actionadmindeleteuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to delete
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDeleteUserAttributes:
    get:
      summary: Admin Delete User Attributes
      description: Deletes the user attributes in a user pool as an administrator.
      operationId: adminDeleteUserAttributes
      x-api-path-slug: actionadmindeleteuserattributes-get
      parameters:
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      - in: query
        name: Username
        description: The user name of the user from which you would like to delete
          attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminDisableUser:
    get:
      summary: Admin Disable User
      description: Disables the specified user as an administrator.
      operationId: adminDisableUser
      x-api-path-slug: actionadmindisableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to disable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to disable
          the user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminEnableUser:
    get:
      summary: Admin Enable User
      description: Enables the specified user as an administrator.
      operationId: adminEnableUser
      x-api-path-slug: actionadminenableuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to enable
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to enable the
          user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminGetUser:
    get:
      summary: Admin Get User
      description: Gets the specified user by user name in a user pool as an administrator.
      operationId: adminGetUser
      x-api-path-slug: actionadmingetuser-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to retrieve
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to get information
          about the            user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminListGroupsForUser:
    get:
      summary: Admin List Groups For User
      description: Lists the groups that the user belongs to.
      operationId: adminListGroupsForUser
      x-api-path-slug: actionadminlistgroupsforuser-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the request to list groups
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminRemoveUserFromGroup:
    get:
      summary: Admin Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: adminRemoveUserFromGroup
      x-api-path-slug: actionadminremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminResetUserPassword:
    get:
      summary: Admin Reset User Password
      description: Resets the specified user's password in a user pool as an administrator.
      operationId: adminResetUserPassword
      x-api-path-slug: actionadminresetuserpassword-get
      parameters:
      - in: query
        name: Username
        description: The user name of the user whose password you wish to reset
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to reset the
          users            password
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Passwords
  /?Action=AdminSetUserSettings:
    get:
      summary: Admin Set User Settings
      description: Sets all the user settings for a specified user name.
      operationId: adminSetUserSettings
      x-api-path-slug: actionadminsetusersettings-get
      parameters:
      - in: query
        name: MFAOptions
        description: Specifies the options for MFA (e
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you wish to set user settings
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to set the
          users settings, such            as MFA options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUpdateDeviceStatus:
    get:
      summary: Admin Update Device Status
      description: Updates the device status as an administrator.
      operationId: adminUpdateDeviceStatus
      x-api-path-slug: actionadminupdatedevicestatus-get
      parameters:
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      - in: query
        name: DeviceRememberedStatus
        description: The status indicating whether a device has been remembered or
          not
        type: string
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID&gt;
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUpdateUserAttributes:
    get:
      summary: Admin Update User Attributes
      description: |-
        Updates the specified user's attributes, including developer attributes, as an
                    administrator.
      operationId: adminUpdateUserAttributes
      x-api-path-slug: actionadminupdateuserattributes-get
      parameters:
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you want to update user attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to update user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUserGlobalSignOut:
    get:
      summary: Admin User Global Sign Out
      description: Signs out users from all devices, as an administrator.
      operationId: adminUserGlobalSignOut
      x-api-path-slug: actionadminuserglobalsignout-get
      parameters:
      - in: query
        name: Username
        description: The user name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Global Sign Out
  /?Action=CreateUserImportJob:
    get:
      summary: Create User Import Job
      description: Creates the user import job.
      operationId: createUserImportJob
      x-api-path-slug: actioncreateuserimportjob-get
      parameters:
      - in: query
        name: CloudWatchLogsRoleArn
        description: The role ARN for the Amazon CloudWatch Logging role for the user
          import            job
        type: string
      - in: query
        name: JobName
        description: The job name for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=CreateUserPool:
    get:
      summary: Create User Pool
      description: |-
        Creates a new Amazon Cognito user pool and sets the password policy for the
                    pool.
      operationId: createUserPool
      x-api-path-slug: actioncreateuserpool-get
      parameters:
      - in: query
        name: AdminCreateUserConfig
        description: The configuration for AdminCreateUser requests
        type: string
      - in: query
        name: AliasAttributes
        description: Attributes supported as an alias for this user pool
        type: string
      - in: query
        name: AutoVerifiedAttributes
        description: The attributes to be auto-verified
        type: string
      - in: query
        name: DeviceConfiguration
        description: The device configuration
        type: string
      - in: query
        name: EmailConfiguration
        description: The email configuration
        type: string
      - in: query
        name: EmailVerificationMessage
        description: A string representing the email verification message
        type: string
      - in: query
        name: EmailVerificationSubject
        description: A string representing the email verification subject
        type: string
      - in: query
        name: LambdaConfig
        description: The Lambda trigger configuration information for the new user
          pool
        type: string
      - in: query
        name: MfaConfiguration
        description: Specifies MFA configuration details
        type: string
      - in: query
        name: Policies
        description: The policies associated with the new user pool
        type: string
      - in: query
        name: PoolName
        description: A string used to name the user pool
        type: string
      - in: query
        name: Schema
        description: An array of schema attributes for the new user pool
        type: string
      - in: query
        name: SmsAuthenticationMessage
        description: A string representing the SMS authentication message
        type: string
      - in: query
        name: SmsConfiguration
        description: The SMS configuration
        type: string
      - in: query
        name: SmsVerificationMessage
        description: A string representing the SMS verification message
        type: string
      - in: query
        name: UserPoolTags
        description: The cost allocation tags for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=CreateUserPoolClient:
    get:
      summary: Create User Pool Client
      description: Creates the user pool client.
      operationId: createUserPoolClient
      x-api-path-slug: actioncreateuserpoolclient-get
      parameters:
      - in: query
        name: ClientName
        description: The client name for the user pool client you would like to create
        type: string
      - in: query
        name: ExplicitAuthFlows
        description: The explicit authentication flows
        type: string
      - in: query
        name: GenerateSecret
        description: Boolean to specify whether you want to generate a secret for
          the user pool client            being created
        type: string
      - in: query
        name: ReadAttributes
        description: The read attributes
        type: string
      - in: query
        name: RefreshTokenValidity
        description: The validity of the refresh token, in days
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to create a
          user pool            client
        type: string
      - in: query
        name: WriteAttributes
        description: The write attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=DeleteUser:
    get:
      summary: Delete User
      description: Allows a user to delete one's self.
      operationId: deleteUser
      x-api-path-slug: actiondeleteuser-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token from a request to delete a user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUserAttributes:
    get:
      summary: Delete User Attributes
      description: Deletes the attributes for a user.
      operationId: deleteUserAttributes
      x-api-path-slug: actiondeleteuserattributes-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token used in the request to delete user attributes
        type: string
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUserPool:
    get:
      summary: Delete User Pool
      description: Deletes the specified Amazon Cognito user pool.
      operationId: deleteUserPool
      x-api-path-slug: actiondeleteuserpool-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DeleteUserPoolClient:
    get:
      summary: Delete User Pool Client
      description: Allows the developer to delete the user pool client.
      operationId: deleteUserPoolClient
      x-api-path-slug: actiondeleteuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete the
          client
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DescribeUserImportJob:
    get:
      summary: Describe User Import Job
      description: Describes the user import job.
      operationId: describeUserImportJob
      x-api-path-slug: actiondescribeuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=DescribeUserPool:
    get:
      summary: Describe User Pool
      description: |-
        Returns the configuration information and metadata of the specified user
                    pool.
      operationId: describeUserPool
      x-api-path-slug: actiondescribeuserpool-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=DescribeUserPoolClient:
    get:
      summary: Describe User Pool Client
      description: |-
        Client method for returning the configuration information and metadata of the
                    specified user pool client.
      operationId: describeUserPoolClient
      x-api-path-slug: actiondescribeuserpoolclient-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pool Clients
  /?Action=GetDevice:
    get:
      summary: Get Device
      description: Gets the device.
      operationId: getDevice
      x-api-path-slug: actiongetdevice-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token
        type: string
      - in: query
        name: DeviceKey
        description: The device key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
  /?Action=GetUser:
    get:
      summary: Get User
      description: Gets the user attributes and metadata for a user.
      operationId: getUser
      x-api-path-slug: actiongetuser-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token returned by the server response to get information
          about the            user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=ListUserImportJobs:
    get:
      summary: List User Import Jobs
      description: Lists the user import jobs.
      operationId: listUserImportJobs
      x-api-path-slug: actionlistuserimportjobs-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of import jobs you want the request to return
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to ListUserImportJobs,
          which            can be used to return the next set of import jobs in the
          list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=ListUsers:
    get:
      summary: List Users
      description: Lists the users in the Amazon Cognito user pool.
      operationId: listUsers
      x-api-path-slug: actionlistusers-get
      parameters:
      - in: query
        name: AttributesToGet
        description: The attributes to get from the request to list users
        type: string
      - in: query
        name: Filter
        description: The filter for the list users request
        type: string
      - in: query
        name: Limit
        description: The limit of the request to list users
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for which you want to list users
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=ListUsersInGroup:
    get:
      summary: List Users In Group
      description: Lists the users in the specified group.
      operationId: listUsersInGroup
      x-api-path-slug: actionlistusersingroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Limit
        description: The limit of the request to list users
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=SetUserSettings:
    get:
      summary: Set User Settings
      description: Sets the user settings like multi-factor authentication (MFA).
      operationId: setUserSettings
      x-api-path-slug: actionsetusersettings-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the set user settings request
        type: string
      - in: query
        name: MFAOptions
        description: Specifies the options for MFA (e
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=StartUserImportJob:
    get:
      summary: Start User Import Job
      description: Starts the user import.
      operationId: startUserImportJob
      x-api-path-slug: actionstartuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Imports
  /?Action=StopUserImportJob:
    get:
      summary: Stop User Import Job
      description: Stops the user import job.
      operationId: stopUserImportJob
      x-api-path-slug: actionstopuserimportjob-get
      parameters:
      - in: query
        name: JobId
        description: The job ID for the user import job
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Iimport
  /?Action=UpdateUserAttributes:
    get:
      summary: Update User Attributes
      description: Allows a user to update a specific attribute (one at a time).
      operationId: updateUserAttributes
      x-api-path-slug: actionupdateuserattributes-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the request to update user attributes
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=UpdateUserPool:
    get:
      summary: Update User Pool
      description: Updates the specified user pool with the specified attributes.
      operationId: updateUserPool
      x-api-path-slug: actionupdateuserpool-get
      parameters:
      - in: query
        name: AdminCreateUserConfig
        description: The configuration for AdminCreateUser requests
        type: string
      - in: query
        name: AutoVerifiedAttributes
        description: The attributes that are automatically verified when the Amazon
          Cognito service            makes a request to update user pools
        type: string
      - in: query
        name: DeviceConfiguration
        description: Device configuration
        type: string
      - in: query
        name: EmailConfiguration
        description: Email configuration
        type: string
      - in: query
        name: EmailVerificationMessage
        description: The contents of the email verification message
        type: string
      - in: query
        name: EmailVerificationSubject
        description: The subject of the email verification message
        type: string
      - in: query
        name: LambdaConfig
        description: The AWS Lambda configuration information from the request to
          update the user            pool
        type: string
      - in: query
        name: MfaConfiguration
        description: 'Can be one of the following values:'
        type: string
      - in: query
        name: Policies
        description: A container with the policies you wish to update in a user pool
        type: string
      - in: query
        name: SmsAuthenticationMessage
        description: The contents of the SMS authentication message
        type: string
      - in: query
        name: SmsConfiguration
        description: SMS configuration
        type: string
      - in: query
        name: SmsVerificationMessage
        description: A container with information about the SMS verification message
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool you want to update
        type: string
      - in: query
        name: UserPoolTags
        description: The cost allocation tags for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Pools
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---