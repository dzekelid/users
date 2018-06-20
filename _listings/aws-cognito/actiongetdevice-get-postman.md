{
  "info": {
    "name": "AWS Cognito API Get Device",
    "_postman_id": "30919391-39ec-4843-9463-801c78fe8516",
    "description": "Gets the device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "febc5762-7076-4dca-9d49-0d2cf8083f76",
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
              "id": "8af714c0-487f-44ce-8c17-0275a859603d"
            }
          ]
        },
        {
          "id": "ab63b837-96ae-468d-9595-31b5e82bb3a2",
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
              "id": "5a48238e-373f-445a-8e1d-02cb4910a742"
            }
          ]
        },
        {
          "id": "b9166b70-96a7-4abd-b71b-8b2c2a251fcf",
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
              "id": "d6a3e2eb-2722-4f3f-9235-4e2a13320f69"
            }
          ]
        },
        {
          "id": "c0dae688-0266-4f36-a120-0313eaad326a",
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
              "id": "18e00d83-b742-4e0e-8e44-c3fd0b335b43"
            }
          ]
        },
        {
          "id": "892c332f-cbd0-4c75-b404-ac29087603b6",
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
              "id": "6cc72969-ab52-480b-9138-ed604890e940"
            }
          ]
        }
      ]
    }
  ]
}