{
  "info": {
    "name": "AWS Directory Service API Create Snapshot",
    "_postman_id": "fc644327-75ec-473d-84ac-420e5c07ee7b",
    "description": "Creates a snapshot of a Simple AD or Microsoft AD directory in the AWS cloud.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "b74ebbe6-4dc8-4f48-a616-ebc2414f659c",
          "name": "addIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=AddIpRoutes?DirectoryId=DirectoryId&IpRoutes=IpRoutes&UpdateSecurityGroupForDirectoryControllers=UpdateSecurityGroupForDirectoryControllers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If the DNS server for your on-premises domain uses a publicly addressable IP address, you must add a CIDR address block to correctly route traffic to and from your Microsoft AD on Amazon Web Services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f791d458-c7df-47cf-8c16-dba29ebd67f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "887c9ddd-e6da-47d6-9db4-2a1b5c500db5",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42c7091a-b55a-4e0a-9b07-7d2b05040b81"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "1bab94ba-d296-4abe-bd96-f20cae5da18e",
          "name": "cancelSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=CancelSchemaExtension?DirectoryId=DirectoryId&SchemaExtensionId=SchemaExtensionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an in-progress schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9727c2c9-64ad-4a15-9e28-8bbcf8721d81"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "62734bea-2c12-4bd9-a086-fe5e49e3485f",
          "name": "connectDirectory",
          "request": {
            "url": "http://example.com/api/?Action=ConnectDirectory?ConnectSettings=ConnectSettings&Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AD Connector to connect to an on-premises directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16e46ae6-44a1-48a6-87be-651ffd3e2564"
            }
          ]
        },
        {
          "id": "a4470b54-ecbd-467b-9785-bbfa0cb12e33",
          "name": "createDirectory",
          "request": {
            "url": "http://example.com/api/?Action=CreateDirectory?Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Simple AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fe452d5-e09a-4146-aa14-07f1ad2bc8b1"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "d3e4618f-4025-48b7-ad29-202cc8ac3d14",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?Alias=Alias&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for a directory and assigns the alias to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f436f77b-dcb4-4938-b84a-c5877e1330f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "84c69f70-37fd-4521-b694-76d25d2488e3",
          "name": "createComputer",
          "request": {
            "url": "http://example.com/api/?Action=CreateComputer?ComputerAttributes=ComputerAttributes&ComputerName=ComputerName&DirectoryId=DirectoryId&OrganizationalUnitDistinguishedName=OrganizationalUnitDistinguishedName&Password=Password",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a computer account in the specified directory, and joins the computer to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63fce2a9-8d4b-40c8-a1f9-c91dc4670806"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "22eacdbb-30d1-4b5d-b651-97456095d735",
          "name": "createConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=CreateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a conditional forwarder associated with your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c0a5886-1844-4b53-968f-ef8dbc5a67e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "f374c4a8-1e74-46b7-aff5-7c90ee2e5976",
          "name": "createMicrosoftAD",
          "request": {
            "url": "http://example.com/api/?Action=CreateMicrosoftAD?Description=Description&Name=Name&Password=Password&ShortName=ShortName&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Microsoft AD in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bb8ad38-8f40-491d-bc18-ed3526f774aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "c3723d9d-a890-4e54-ac86-e0ab0ed44999",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?DirectoryId=DirectoryId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a Simple AD or Microsoft AD directory in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45ee6298-56c4-4aef-9601-baf3d7c45552"
            }
          ]
        }
      ]
    }
  ]
}