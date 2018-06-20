---
name: AWS Directory Service
x-slug: aws-directory-service
description: AWS Directory Service for Microsoft Active Directory (Enterprise Edition),
  also known as AWS Microsoft AD, enables your directory-aware workloads and AWS resources
  to use managed Active Directory in the AWS Cloud. The Microsoft AD service is built
  on actual Microsoft Active Directory and does not require you to synchronize or
  replicate data from your existing Active Directory to the cloud. You can use standard
  Active Directory administration tools and take advantage of built-in Active Directory
  features such as Group Policy, trusts, and single sign-on. With Microsoft AD, you
  can easily joinAmazon EC2andAmazon RDS for SQL Serverinstances to a domain, and
  useAWS Enterprise IT applicationssuch asAmazon WorkSpaceswith Active Directory users
  and groups.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Snapshots
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-directory-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Directory Service API Delete Snapshot
  x-api-slug: aws-directory-service-api
  description: Deletes a directory snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
  humanURL: https://aws.amazon.com/directoryservice/
  baseURL: ://///?Action=DeleteSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-directory-service/actiondeletesnapshot-get-openapi.md
- name: AWS Directory Service API Describe Snapshots
  x-api-slug: aws-directory-service-api
  description: Obtains information about the directory snapshots that belong to this
    account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
  humanURL: https://aws.amazon.com/directoryservice/
  baseURL: ://///?Action=DescribeSnapshots
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-directory-service/actiondescribesnapshots-get-openapi.md
- name: AWS Directory Service API Get Snapshot Limits
  x-api-slug: aws-directory-service-api
  description: Obtains the manual snapshot limits for a directory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
  humanURL: https://aws.amazon.com/directoryservice/
  baseURL: ://///?Action=GetSnapshotLimits
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-directory-service/actiongetsnapshotlimits-get-openapi.md
- name: AWS Directory Service API Restore From Snapshot
  x-api-slug: aws-directory-service-api
  description: Restores a directory using an existing directory snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
  humanURL: https://aws.amazon.com/directoryservice/
  baseURL: ://///?Action=RestoreFromSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-directory-service/actionrestorefromsnapshot-get-openapi.md
- name: AWS Directory Service API
  x-api-slug: aws-directory-service-api
  description: AWS Directory Service for Microsoft Active Directory (Enterprise Edition),
    also known as AWS Microsoft AD, enables your directory-aware workloads and AWS
    resources to use managed Active Directory in the AWS Cloud. The Microsoft AD service
    is built on actual Microsoft Active Directory and does not require you to synchronize
    or replicate data from your existing Active Directory to the cloud. You can use
    standard Active Directory administration tools and take advantage of built-in
    Active Directory features such as Group Policy, trusts, and single sign-on. With
    Microsoft AD, you can easily joinAmazon EC2andAmazon RDS for SQL Serverinstances
    to a domain, and useAWS Enterprise IT applicationssuch asAmazon WorkSpaceswith
    Active Directory users and groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSDirectoryService.png
  humanURL: https://aws.amazon.com/directoryservice/
  baseURL: :///
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-directory-service/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/ds/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/directoryservice/latest/devguide/api-ref.html
- type: x-faq
  url: https://aws.amazon.com/directoryservice/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/directoryservice/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/directoryservice/pricing/
- type: x-website
  url: https://aws.amazon.com/directoryservice/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---