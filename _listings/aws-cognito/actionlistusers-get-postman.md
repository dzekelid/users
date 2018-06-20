{
  "info": {
    "name": "AWS Cognito API List Users",
    "_postman_id": "8023def8-698d-4636-8c07-cf74e01fd9cf",
    "description": "Lists the users in the Amazon Cognito user pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes",
      "item": [
        {
          "id": "f3da06db-7bd3-463e-bc8a-588370ed748c",
          "name": "addCustomAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AddCustomAttributes?CustomAttributes=CustomAttributes&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds additional user attributes to the user pool schema."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ce83291-a3e9-4d19-afe6-28c49684e1fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "f085921f-f836-4b5b-a451-6ee7425bdc28",
          "name": "adminAddUserToGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminAddUserToGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified user to the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92baec76-c58b-43ca-bdad-cec31aacad11"
            }
          ]
        },
        {
          "id": "12f73d90-9cb6-4403-8b3f-4e191d45a018",
          "name": "adminCreateUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminCreateUser?DesiredDeliveryMediums=DesiredDeliveryMediums&ForceAliasCreation=ForceAliasCreation&MessageAction=MessageAction&TemporaryPassword=TemporaryPassword&UserAttributes=UserAttributes&Username=Username&UserPoolId=UserPoolId&ValidationData=ValidationData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new user in the specified user pool and sends a welcome message via email\n            or phone (SMS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71cf5ce0-8da3-4377-b1dc-caa59308af0b"
            }
          ]
        },
        {
          "id": "369d47e7-00d2-444b-a4ab-f2f62ed27405",
          "name": "adminDeleteUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminDeleteUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3515945b-593e-444f-a07f-ccfd9dc3ec78"
            }
          ]
        },
        {
          "id": "2d987d7d-9314-4eb0-a4b8-da8889d18b81",
          "name": "adminDeleteUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AdminDeleteUserAttributes?UserAttributeNames=UserAttributeNames&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the user attributes in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7f0b580-96ea-4c93-b865-a6949383192e"
            }
          ]
        },
        {
          "id": "a62f59fb-a2e0-4c80-9714-441efc01cdc2",
          "name": "adminDisableUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminDisableUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables the specified user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5f2843d-93dd-482a-8174-57c7de33f809"
            }
          ]
        },
        {
          "id": "7eafd400-6e67-4c8a-9bfd-1e2b055d3afb",
          "name": "adminEnableUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminEnableUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the specified user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83fc6a58-5acd-4607-8a72-899111c537b9"
            }
          ]
        },
        {
          "id": "a601a3a0-95f9-4e77-8736-8e699d98306e",
          "name": "adminGetUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminGetUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified user by user name in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6deb5414-98eb-4124-ab41-1b88cf02a6b2"
            }
          ]
        },
        {
          "id": "c5b73bb2-55fe-43b1-9739-2fe41b77754c",
          "name": "adminListGroupsForUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminListGroupsForUser?Limit=Limit&NextToken=NextToken&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the groups that the user belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bdcbccc-4f46-48de-afa1-65fe202c8708"
            }
          ]
        },
        {
          "id": "33c088ba-19c6-43a4-9aab-c7cee4851b78",
          "name": "adminRemoveUserFromGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminRemoveUserFromGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified user from the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52c64baf-31cb-4c8f-b64f-81d87d73a39f"
            }
          ]
        },
        {
          "id": "983e1647-a79b-4575-aab2-f788adbfcf35",
          "name": "adminResetUserPassword",
          "request": {
            "url": "http://example.com/api/?Action=AdminResetUserPassword?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resets the specified user's password in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cab09ae5-1353-4ac3-832e-fb3ac560b2d9"
            }
          ]
        },
        {
          "id": "7785321a-4f79-4906-aa8a-ad39c11d987d",
          "name": "adminSetUserSettings",
          "request": {
            "url": "http://example.com/api/?Action=AdminSetUserSettings?MFAOptions=MFAOptions&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets all the user settings for a specified user name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccfeaa7b-5388-43e7-a032-f6c95e431ab8"
            }
          ]
        },
        {
          "id": "03ac059f-8ffc-40f0-8556-cc4c16ef4c5d",
          "name": "adminUpdateDeviceStatus",
          "request": {
            "url": "http://example.com/api/?Action=AdminUpdateDeviceStatus?DeviceKey=DeviceKey&DeviceRememberedStatus=DeviceRememberedStatus&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the device status as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a86e800a-1b77-478a-bbb2-778a12c01212"
            }
          ]
        },
        {
          "id": "5a7672c1-86c7-4d77-82bf-bd0b0b2df9e8",
          "name": "adminUpdateUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AdminUpdateUserAttributes?UserAttributes=UserAttributes&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified user's attributes, including developer attributes, as an\n            administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fab1d842-49fb-4aa7-abc6-5b18db543cb3"
            }
          ]
        },
        {
          "id": "41cb6a9d-7398-417a-bb54-f8addf6e17f7",
          "name": "adminUserGlobalSignOut",
          "request": {
            "url": "http://example.com/api/?Action=AdminUserGlobalSignOut?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Signs out users from all devices, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d74e6dae-2821-48ca-b244-644d5d432ca5"
            }
          ]
        },
        {
          "id": "574a0eb6-4ff1-4fb0-9224-f0402dd29e7b",
          "name": "createUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserImportJob?CloudWatchLogsRoleArn=CloudWatchLogsRoleArn&JobName=JobName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b58f734-0067-45b1-98b4-acf515735ded"
            }
          ]
        },
        {
          "id": "d01644d9-61e9-406a-b22a-9c6a7ef95bf1",
          "name": "createUserPool",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AliasAttributes=AliasAttributes&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&PoolName=PoolName&Schema=Schema&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Cognito user pool and sets the password policy for the\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee42bd7e-5661-4f6d-8879-8961f5e56c3d"
            }
          ]
        },
        {
          "id": "ec1fb812-4528-4ccf-bec3-d8b4c7a24c01",
          "name": "createUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPoolClient?ClientName=ClientName&ExplicitAuthFlows=ExplicitAuthFlows&GenerateSecret=GenerateSecret&ReadAttributes=ReadAttributes&RefreshTokenValidity=RefreshTokenValidity&UserPoolId=UserPoolId&WriteAttributes=WriteAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39159d26-bc85-4e6a-9d46-d25654c3a554"
            }
          ]
        },
        {
          "id": "52028ff8-1aa5-495f-a9b8-5cfef1614e91",
          "name": "deleteUser",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUser?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to delete one's self."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de8f6a8b-c9ca-4b6d-b172-7cdec8ccb41a"
            }
          ]
        },
        {
          "id": "872a3474-e7e4-4c55-9dfc-dbf8e64f699b",
          "name": "deleteUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserAttributes?AccessToken=AccessToken&UserAttributeNames=UserAttributeNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the attributes for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd08f992-d91c-474d-b9da-a881293066a0"
            }
          ]
        },
        {
          "id": "8515220d-8c53-4a7a-8516-2acd4055e1a0",
          "name": "deleteUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d733d951-3dd4-423a-91dd-742b1bfc4401"
            }
          ]
        },
        {
          "id": "6a61c9da-4901-477d-934d-ce01e3f36525",
          "name": "deleteUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the developer to delete the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5b5cb36-8dc2-4068-b8ef-312fb8461dc5"
            }
          ]
        },
        {
          "id": "1b626583-9265-422b-b7e1-01d0543bea72",
          "name": "describeUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserImportJob?JobId=JobId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "353a4a51-a1b0-4ed2-98be-c46016138f0a"
            }
          ]
        },
        {
          "id": "a24dca04-3cd3-4578-9f4a-7ab0eaa45287",
          "name": "describeUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information and metadata of the specified user\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c31e76ea-6b48-48ae-af78-1bb396e01e67"
            }
          ]
        },
        {
          "id": "4914d7ad-30bb-4452-87f6-17baee845e4a",
          "name": "describeUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Client method for returning the configuration information and metadata of the\n            specified user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bede1a41-ade3-40e7-9c69-033f4a8167cd"
            }
          ]
        },
        {
          "id": "d68de19d-470c-4605-ad45-73edc37f2daa",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4feaf59d-91d5-4999-bd6a-fb905a7d97b7"
            }
          ]
        },
        {
          "id": "4afe8c5f-d51d-4e4c-947f-c992a7f1fe12",
          "name": "getUser",
          "request": {
            "url": "http://example.com/api/?Action=GetUser?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the user attributes and metadata for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72f60de9-eeb8-48c3-9e78-e025e3b724a9"
            }
          ]
        },
        {
          "id": "0a19a7a6-30b6-4508-afd1-a2c2e257a025",
          "name": "listUserImportJobs",
          "request": {
            "url": "http://example.com/api/?Action=ListUserImportJobs?MaxResults=MaxResults&PaginationToken=PaginationToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the user import jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3bab9f0-58dd-4b27-9634-e423e313a9a4"
            }
          ]
        },
        {
          "id": "b4dee946-a5ae-4c41-8071-68fbd44b1c85",
          "name": "listUsers",
          "request": {
            "url": "http://example.com/api/?Action=ListUsers?AttributesToGet=AttributesToGet&Filter=Filter&Limit=Limit&PaginationToken=PaginationToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the users in the Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "435a9b16-6a2c-41e9-ae33-713929999e9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Up",
      "item": [
        {
          "id": "4c1a1611-1cec-45e9-8a01-cd61d8f0ed06",
          "name": "adminConfirmSignUp",
          "request": {
            "url": "http://example.com/api/?Action=AdminConfirmSignUp?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms user registration as an admin without using a confirmation code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14a28cf2-34f7-49f6-9ed3-e7138656cc2a"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "733f2de1-d82d-45fc-9914-2fa88951991a",
          "name": "adminForgetDevice",
          "request": {
            "url": "http://example.com/api/?Action=AdminForgetDevice?DeviceKey=DeviceKey&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forgets the device, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb23b189-2522-43ab-8035-6546fcab4267"
            }
          ]
        },
        {
          "id": "f8680ed9-a587-4092-a5d9-78bea8ad179a",
          "name": "confirmDevice",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmDevice?AccessToken=AccessToken&DeviceKey=DeviceKey&DeviceName=DeviceName&DeviceSecretVerifierConfig=DeviceSecretVerifierConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms tracking of the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c52d524-7a63-4ab5-b7df-b66516d3f2f1"
            }
          ]
        },
        {
          "id": "69e16937-9f67-4351-a102-8107e294f934",
          "name": "forgetDevice",
          "request": {
            "url": "http://example.com/api/?Action=ForgetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forgets the specified device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0f49e67-c56c-4e98-87db-3efeb15eaa21"
            }
          ]
        },
        {
          "id": "be4c690e-5177-4387-9767-0538bc768702",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?AccessToken=AccessToken&Limit=Limit&PaginationToken=PaginationToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1430738-4b06-4bb8-b675-4cba93842174"
            }
          ]
        }
      ]
    },
    {
      "name": "http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php",
      "item": [
        {
          "id": "b74dc348-44a7-4f92-bcf8-e957cbde60e1",
          "name": "adminGetDevice",
          "request": {
            "url": "http://example.com/api/?Action=AdminGetDevice?DeviceKey=DeviceKey&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbc35c49-1fea-485a-b72b-637d5bc4fa0a"
            }
          ]
        },
        {
          "id": "3b231f76-a1d1-49c8-afcd-af84b5e34e36",
          "name": "adminListDevices",
          "request": {
            "url": "http://example.com/api/?Action=AdminListDevices?Limit=Limit&PaginationToken=PaginationToken&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists devices, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccb3328d-6c15-4998-bf83-cce2ea7c6059"
            }
          ]
        }
      ]
    },
    {
      "name": "Authnetication",
      "item": [
        {
          "id": "7a616bb3-4cef-4a90-b385-bd869c3ee7c3",
          "name": "adminInitiateAuth",
          "request": {
            "url": "http://example.com/api/?Action=AdminInitiateAuth?AuthFlow=AuthFlow&AuthParameters=AuthParameters&ClientId=ClientId&ClientMetadata=ClientMetadata&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the authentication flow, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "840a18c8-018d-47a3-b0a4-62578148edf9"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication Challenge",
      "item": [
        {
          "id": "ade6d906-288f-4bbb-b33c-0bd78fa0d878",
          "name": "adminRespondToAuthChallenge",
          "request": {
            "url": "http://example.com/api/?Action=AdminRespondToAuthChallenge?ChallengeName=ChallengeName&ChallengeResponses=ChallengeResponses&ClientId=ClientId&Session=Session&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Responds to an authentication challenge, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cd023b4-46c9-4d85-82c7-94ca0fe279de"
            }
          ]
        }
      ]
    },
    {
      "name": "Password",
      "item": [
        {
          "id": "075b47b8-72df-412c-89a1-73dcc1a012d1",
          "name": "changePassword",
          "request": {
            "url": "http://example.com/api/?Action=ChangePassword?AccessToken=AccessToken&PreviousPassword=PreviousPassword&ProposedPassword=ProposedPassword",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password for a specified user in a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72db48a5-0e41-486a-b0f3-7312717f75dd"
            }
          ]
        }
      ]
    },
    {
      "name": "Passwords",
      "item": [
        {
          "id": "04145ba2-c13d-4124-819c-856dfca4106c",
          "name": "confirmForgotPassword",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmForgotPassword?ClientId=ClientId&ConfirmationCode=ConfirmationCode&Password=Password&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to enter a code provided when they reset their password to update\n            their password."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "954911ed-365e-40bb-b553-0515fe219e92"
            }
          ]
        },
        {
          "id": "75d10970-8e7e-450a-b603-a09a58cb03da",
          "name": "forgotPassword",
          "request": {
            "url": "http://example.com/api/?Action=ForgotPassword?ClientId=ClientId&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the password for the specified client ID or username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3252ec5e-2132-4e5d-829a-2beb7506f371"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Ups",
      "item": [
        {
          "id": "9c333197-6559-47e4-b7be-bf5947abd350",
          "name": "confirmSignUp",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSignUp?ClientId=ClientId&ConfirmationCode=ConfirmationCode&ForceAliasCreation=ForceAliasCreation&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms registration of a user and handles the existing alias from a previous\n            user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ff35775-14e2-4952-9a47-9da0fe4f0aff"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "538c1eca-0508-41f3-a393-f328c547cb7a",
          "name": "createGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateGroup?Description=Description&GroupName=GroupName&Precedence=Precedence&RoleArn=RoleArn&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new group in the specified user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05379df7-7a53-4ee5-994f-2eb0823d8bb7"
            }
          ]
        },
        {
          "id": "0a5fd4b1-da78-40bf-8c8b-b918429f5a37",
          "name": "deleteGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGroup?GroupName=GroupName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d202a426-20af-4570-80e1-5c69afb00f46"
            }
          ]
        },
        {
          "id": "cbbbfc92-e3ab-44b1-ad70-5a95034f2ac0",
          "name": "getGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetGroup?GroupName=GroupName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09075fe0-2782-4249-890c-0d0ce52e7218"
            }
          ]
        },
        {
          "id": "3327da95-07e6-4c7f-97dc-09eaeb39398c",
          "name": "listGroups",
          "request": {
            "url": "http://example.com/api/?Action=ListGroups?Limit=Limit&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the groups associated with a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ceed631-c7e4-4f41-90d7-c4976ef90764"
            }
          ]
        }
      ]
    },
    {
      "name": "CSV Header",
      "item": [
        {
          "id": "53aa5368-c37e-4a65-8aab-14964b567c96",
          "name": "getCSVHeader",
          "request": {
            "url": "http://example.com/api/?Action=GetCSVHeader?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the header information for the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0663bb6-e29e-4455-a733-40a8e1e294da"
            }
          ]
        }
      ]
    },
    {
      "name": "Verification Codes",
      "item": [
        {
          "id": "a970dcc3-1313-46f7-9771-25f3a279bfd3",
          "name": "getUserAttributeVerificationCode",
          "request": {
            "url": "http://example.com/api/?Action=GetUserAttributeVerificationCode?AccessToken=AccessToken&AttributeName=AttributeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the user attribute verification code for the specified attribute\n            name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8010cb8d-7976-48ca-88cf-11e4ada76ae1"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Out",
      "item": [
        {
          "id": "9732a11e-b703-4618-8715-9c06f71b2c9e",
          "name": "globalSignOut",
          "request": {
            "url": "http://example.com/api/?Action=GlobalSignOut?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Signs out users from all devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb16afc8-e3ec-4f66-8fc6-9d6ad2a6f6d7"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication",
      "item": [
        {
          "id": "43473c06-3a6d-4cfd-b9f0-52e63b5e4a8e",
          "name": "initiateAuth",
          "request": {
            "url": "http://example.com/api/?Action=InitiateAuth?AuthFlow=AuthFlow&AuthParameters=AuthParameters&ClientId=ClientId&ClientMetadata=ClientMetadata",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the authentication flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "257abcea-840d-4b8a-9671-7d4af8ab4abc"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pool Clients",
      "item": [
        {
          "id": "fa82e0da-e5af-4fd2-ac59-67cdd7617273",
          "name": "listUserPoolClients",
          "request": {
            "url": "http://example.com/api/?Action=ListUserPoolClients?MaxResults=MaxResults&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the clients that have been created for the specified user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14a80e41-6420-4575-bbd6-a4ef3126ac7c"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pools",
      "item": [
        {
          "id": "1677f0de-ef14-4023-bfd1-32e368ea7c4e",
          "name": "listUserPools",
          "request": {
            "url": "http://example.com/api/?Action=ListUserPools?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the user pools associated with an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d10edd9-f2de-47fc-bed9-b2e6a906134d"
            }
          ]
        }
      ]
    }
  ]
}