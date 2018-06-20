{
  "info": {
    "name": "AWS Cognito API List Users In Group",
    "_postman_id": "c25e6566-f6c8-404c-8c4d-3e0b9e59da35",
    "description": "Lists the users in the specified group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes",
      "item": [
        {
          "id": "e151ee71-934a-4268-ad33-5d6a638c559a",
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
              "id": "bf4fe69e-2348-42cb-bc89-c9b41b5132bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "cd2c94e2-9ce5-4abe-a57b-dd00c0c54119",
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
              "id": "4c8748b8-5db4-4145-825e-124836b269c1"
            }
          ]
        },
        {
          "id": "a127c5da-5066-42a9-b7b0-c635a5b252df",
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
              "id": "3db08312-7bd5-48f1-bcbf-b7ef6e3c21a9"
            }
          ]
        },
        {
          "id": "6b9933da-0b5a-4f67-ab2b-59c760ed8090",
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
              "id": "3b1a993e-4c43-4a98-8523-1a227440bc3d"
            }
          ]
        },
        {
          "id": "afb3aac0-b315-4cd1-97c9-baf22a673acf",
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
              "id": "196241ae-16ee-4769-9335-fb2b1e2033ee"
            }
          ]
        },
        {
          "id": "44f942f5-ad2f-4013-8dc9-526171cb1216",
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
              "id": "a87be692-ca2f-4de3-bcd6-4dbbd4c52fc6"
            }
          ]
        },
        {
          "id": "e22c7f9b-6b8d-42ef-9079-ae846a6b6033",
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
              "id": "87bd5225-2634-4fec-8e8e-12b00ba7ec14"
            }
          ]
        },
        {
          "id": "ea5050ce-e0eb-4cc0-9213-095a0eabae07",
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
              "id": "9787eae6-f7aa-499c-92ad-45edc9170b57"
            }
          ]
        },
        {
          "id": "bc1b2c58-7de9-4e33-ba95-80f5ca6fc6dc",
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
              "id": "abc47d6f-23c9-41ca-82f7-e8a33b923ef4"
            }
          ]
        },
        {
          "id": "a5b327ef-c97c-4af5-a07d-397064b5dffa",
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
              "id": "29b145a3-937d-4169-bcd0-e0d488f96acd"
            }
          ]
        },
        {
          "id": "ac7f6166-5e36-4e16-8010-e105a5dcee24",
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
              "id": "cb9350d1-e441-4383-8723-4f0c2ed07600"
            }
          ]
        },
        {
          "id": "5d4c58db-4cc9-4d3c-ae1d-acc7cb1d62b5",
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
              "id": "912e5b3d-43c8-49b8-afbf-2ff0cb27757f"
            }
          ]
        },
        {
          "id": "505af744-e326-4aa0-89fb-af1eec58ce4c",
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
              "id": "22295575-a58b-4f35-97be-1e54ed874e44"
            }
          ]
        },
        {
          "id": "4451fa02-e4a2-4213-bd70-dbd57844e4c2",
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
              "id": "0f390e2f-d193-42fb-bc7d-eb9aef422e7a"
            }
          ]
        },
        {
          "id": "0c662539-b90e-4e35-88ec-45b800c6224c",
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
              "id": "cfcbebd1-fb85-49f7-86fb-ee7c06bfaf15"
            }
          ]
        },
        {
          "id": "627f367e-85e2-4c61-a6d6-462b064bf6e5",
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
              "id": "bc0dea63-3c84-461f-bb80-67c106ef9d23"
            }
          ]
        },
        {
          "id": "ae4d8231-89d5-4b88-a672-f2e6c7a1a69c",
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
              "id": "8156bf23-e427-49fa-81f1-3f3ce0d1420f"
            }
          ]
        },
        {
          "id": "709c1997-53e9-4c16-ae6f-5f6d622fb0db",
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
              "id": "a8d9c19d-cd73-4459-8c59-abbb52bd28e5"
            }
          ]
        },
        {
          "id": "7a1a4458-5d8c-49fd-9759-415f868fbcb6",
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
              "id": "34a703fb-cb2a-41cc-b3a2-b9b2bd37dbc5"
            }
          ]
        },
        {
          "id": "6d4bcc2d-37b8-40cf-a6c8-b31ee0685724",
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
              "id": "6443d14e-90d8-4600-ae2f-cbfa8499aaa0"
            }
          ]
        },
        {
          "id": "c66a1e0d-b59d-4ed2-b477-c16e7a4ed8c0",
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
              "id": "79de0aaa-8b3a-4e7e-ab05-a3b8bff6d59a"
            }
          ]
        },
        {
          "id": "7bcb8911-816e-4355-8b62-115fcf4c781a",
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
              "id": "d74e3b9f-b356-4097-86b1-008345e91fa7"
            }
          ]
        },
        {
          "id": "51d667f1-1a72-49be-a320-baffafb0dad2",
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
              "id": "76515d6c-a810-4022-be20-cae67c9f71d1"
            }
          ]
        },
        {
          "id": "94287105-1277-4639-b44f-69abb4923e84",
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
              "id": "b9050197-2519-41b8-bbbe-c34d28c83f6c"
            }
          ]
        },
        {
          "id": "593d7b60-20ab-48f6-b5db-e6fa5cc8733c",
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
              "id": "f8e162e2-71d9-4eef-80cf-b301a2115175"
            }
          ]
        },
        {
          "id": "cf862044-b988-4b7e-8612-5d518e6b161b",
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
              "id": "beb5ee72-cf9c-4f91-ad3b-2dcc97b4bbd7"
            }
          ]
        },
        {
          "id": "ba1da699-584c-4aed-ac18-62d88081d240",
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
              "id": "72e26b1b-a32d-4d9d-8896-9b34aaa27d78"
            }
          ]
        },
        {
          "id": "b2244f71-59a2-468e-a8e6-b11105f532c6",
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
              "id": "38a4afc2-76b9-450b-bed4-b53c4c21b7f2"
            }
          ]
        },
        {
          "id": "6e047a89-e3af-49c6-941e-dc2c89e35654",
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
              "id": "2e095b42-1398-4a5b-95d6-b066e27650e2"
            }
          ]
        },
        {
          "id": "640f8893-9748-4b57-96a7-d20dbd189788",
          "name": "listUsersInGroup",
          "request": {
            "url": "http://example.com/api/?Action=ListUsersInGroup?GroupName=GroupName&Limit=Limit&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the users in the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "892a1d99-6655-4891-bee8-0a44bcb99083"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Up",
      "item": [
        {
          "id": "d7769ceb-6675-4ad7-a6ba-d5a551fba521",
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
              "id": "04aa1168-2a65-46e9-80e0-82eecc25ee43"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "00ef599a-8aef-4a9c-b359-72a76d10aa46",
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
              "id": "265c296d-91fc-4120-8159-c71bee2d9986"
            }
          ]
        },
        {
          "id": "39f2fc32-424a-4e21-8722-4b0ee5fc499d",
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
              "id": "ce549942-bb36-486f-8c0e-1aa802f9b180"
            }
          ]
        },
        {
          "id": "758e3e16-7190-4b74-ba43-63d28fe19afe",
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
              "id": "d7f5630d-fa91-4ee3-ae02-25fb564bc564"
            }
          ]
        },
        {
          "id": "ae24433a-c7da-4d4a-a42b-915eed623a31",
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
              "id": "164a8d1a-ced9-417b-9078-3ccca8c86c9b"
            }
          ]
        }
      ]
    },
    {
      "name": "http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php",
      "item": [
        {
          "id": "bebdd74a-8929-4f14-8dbb-fb8b7ff7a0d4",
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
              "id": "fba967aa-ef7c-481a-84e7-b24bca4b9894"
            }
          ]
        },
        {
          "id": "2c8024c3-396d-4b3c-8e7e-a92ed98fb794",
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
              "id": "5c31fa2e-5786-4769-aaeb-e91d5ed37540"
            }
          ]
        }
      ]
    },
    {
      "name": "Authnetication",
      "item": [
        {
          "id": "57a7fc41-fda8-4435-af60-69e0dc5f89b3",
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
              "id": "d0cbdcdc-5b35-41b1-853a-fe82b79516c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication Challenge",
      "item": [
        {
          "id": "f5c6ff59-620c-4c15-9df7-e41ade0ac6d2",
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
              "id": "40ed1e0a-512d-47c9-9866-ee244b02fe35"
            }
          ]
        }
      ]
    },
    {
      "name": "Password",
      "item": [
        {
          "id": "8a98363b-9167-469a-bb6d-927e6ca77477",
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
              "id": "7d1a378e-179d-474b-b6bb-d14f1406a164"
            }
          ]
        }
      ]
    },
    {
      "name": "Passwords",
      "item": [
        {
          "id": "4bc1166e-cb72-40a9-83ac-4db4759061ea",
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
              "id": "d244389a-1664-43e0-8c31-52bd33842efc"
            }
          ]
        },
        {
          "id": "e27be479-06d3-49bc-ac3a-112a7d26c24e",
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
              "id": "268b4a26-467b-4c6e-bf4c-494a48c6701a"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Ups",
      "item": [
        {
          "id": "ed8a268b-7ef3-43f2-aa29-f3bf0c783f3b",
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
              "id": "02abcb47-2042-4bc3-92d3-3da8522234b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "28e84113-b14c-47f3-be38-1e1b83a4c23d",
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
              "id": "6539f7a6-8a68-4b18-a7ad-4ad568947d16"
            }
          ]
        },
        {
          "id": "68a82e40-143a-4f3f-ad4b-58f3f3f91238",
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
              "id": "83e91054-db72-405e-adc5-d7569d2436c4"
            }
          ]
        },
        {
          "id": "30ec449f-3f32-4a5d-897c-ca364bcb8bd4",
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
              "id": "1ca8e470-e635-45f9-96ab-cf03dcf199eb"
            }
          ]
        },
        {
          "id": "a32003db-d150-412f-a6c6-da021efec4ac",
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
              "id": "35d752a9-aa7e-4546-858f-052075257e90"
            }
          ]
        }
      ]
    },
    {
      "name": "CSV Header",
      "item": [
        {
          "id": "db421ee2-f552-421c-9fed-e1c167265358",
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
              "id": "85072b15-e87a-4b52-9839-7abeaeaf80ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Verification Codes",
      "item": [
        {
          "id": "9bd66c63-caa7-4eaa-9a82-911e07b95683",
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
              "id": "bd890ae6-7ccc-4f94-9cf6-4fe6e2860317"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Out",
      "item": [
        {
          "id": "6fa8596b-3fa0-40d4-b8c8-ba4ff836302e",
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
              "id": "827a25c1-fb2f-4722-a527-a4bf4d685c26"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication",
      "item": [
        {
          "id": "9a442478-cc2a-4fa8-8a55-f828678b9448",
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
              "id": "0e09f4c8-27ec-4acf-984f-4d0b5103b54a"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pool Clients",
      "item": [
        {
          "id": "ba7c9ba7-2fcc-4547-8f24-9785056d30bb",
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
              "id": "d7a56d68-2bf2-4880-ace7-2b42dd03674d"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pools",
      "item": [
        {
          "id": "627caba2-5b7b-41d4-954c-daa770254b5f",
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
              "id": "fe93a0bd-23b3-4181-b7fc-5b6fb2e427e9"
            }
          ]
        }
      ]
    }
  ]
}