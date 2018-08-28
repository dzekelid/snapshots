---
name: AWS EC2
x-slug: aws-ec2
description: Amazon Elastic Compute Cloud is a web service that provides resizable
  compute capacity in the cloud. It is designed to make web-scale cloud computing
  easier for developers. Amazon EC2s simple web service interface allows you to obtain
  and configure capacity with minimal friction. It provides you with complete control
  of your computing resources and lets you run on Amazon&rsquo;s proven computing
  environment. Amazon EC2 reduces the time required to obtain and boot new server
  instances to minutes, allowing you to quickly scale capacity, both up and down,
  as your computing requirements change. Amazon EC2 changes the economics of computing
  by allowing you to pay only for capacity that you actually use. Amazon EC2 provides
  developers the tools to build failure resilient applications and isolate themselves
  from common failure scenarios.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Snapshots
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/apis.md
specificationVersion: "0.14"
apis:
- name: AWS EC2 API - Create Snapshot
  x-api-slug: actioncreatesnapshot-get
  description: Creates a snapshot of an EBS volume and stores it in Amazon S3.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncreatesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncreatesnapshot-get-openapi.md
- name: AWS EC2 API - Delete Snapshot
  x-api-slug: actiondeletesnapshot-get
  description: Deletes the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondeletesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondeletesnapshot-get-openapi.md
- name: AWS EC2 API - Modify Snapshot Attribute
  x-api-slug: actionmodifysnapshotattribute-get
  description: Adds or removes permission settings for the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionmodifysnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionmodifysnapshotattribute-get-openapi.md
- name: AWS EC2 API - Reset Snapshot Attribute
  x-api-slug: actionresetsnapshotattribute-get
  description: Resets permission settings for the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionresetsnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionresetsnapshotattribute-get-openapi.md
- name: AWS EC2 API - Import Snapshot
  x-api-slug: actionimportsnapshot-get
  description: Describes your import snapshot tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionimportsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionimportsnapshot-get-openapi.md
- name: AWS EC2 API - Describe Snapshots
  x-api-slug: actiondescribesnapshots-get
  description: Describes one or more of the EBS snapshots available to you.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribesnapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribesnapshots-get-openapi.md
- name: AWS EC2 API - Create Snapshot
  x-api-slug: actioncreatesnapshot-get
  description: Creates a snapshot of an EBS volume and stores it in Amazon S3.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncreatesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncreatesnapshot-get-openapi.md
- name: AWS EC2 API - Delete Snapshot
  x-api-slug: actiondeletesnapshot-get
  description: Deletes the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondeletesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondeletesnapshot-get-openapi.md
- name: AWS EC2 API - Modify Snapshot Attribute
  x-api-slug: actionmodifysnapshotattribute-get
  description: Adds or removes permission settings for the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionmodifysnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionmodifysnapshotattribute-get-openapi.md
- name: AWS EC2 API - Reset Snapshot Attribute
  x-api-slug: actionresetsnapshotattribute-get
  description: Resets permission settings for the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionresetsnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionresetsnapshotattribute-get-openapi.md
- name: AWS EC2 API - Import Snapshot
  x-api-slug: actionimportsnapshot-get
  description: Describes your import snapshot tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionimportsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionimportsnapshot-get-openapi.md
- name: AWS EC2 API - Copy Snapshot
  x-api-slug: actioncopysnapshot-get
  description: Copies a point-in-time snapshot of an EBS volume and stores it in Amazon
    S3.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncopysnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncopysnapshot-get-openapi.md
- name: AWS EC2 API - Describe Import Snapshot Tasks
  x-api-slug: actiondescribeimportsnapshottasks-get
  description: Describes your import snapshot tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribeimportsnapshottasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribeimportsnapshottasks-get-openapi.md
- name: AWS EC2 API - Describe Snapshot Attribute
  x-api-slug: actiondescribesnapshotattribute-get
  description: Describes the specified attribute of the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribesnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribesnapshotattribute-get-openapi.md
- name: AWS EC2 API - Describe Snapshots
  x-api-slug: actiondescribesnapshots-get
  description: Describes one or more of the EBS snapshots available to you.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribesnapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondescribesnapshots-get-openapi.md
- name: AWS EC2 API - Create Snapshot
  x-api-slug: actioncreatesnapshot-get
  description: Creates a snapshot of an EBS volume and stores it in Amazon S3.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncreatesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actioncreatesnapshot-get-openapi.md
- name: AWS EC2 API - Delete Snapshot
  x-api-slug: actiondeletesnapshot-get
  description: Deletes the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondeletesnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actiondeletesnapshot-get-openapi.md
- name: AWS EC2 API - Modify Snapshot Attribute
  x-api-slug: actionmodifysnapshotattribute-get
  description: Adds or removes permission settings for the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionmodifysnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionmodifysnapshotattribute-get-openapi.md
- name: AWS EC2 API - Reset Snapshot Attribute
  x-api-slug: actionresetsnapshotattribute-get
  description: Resets permission settings for the specified snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionresetsnapshotattribute-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionresetsnapshotattribute-get-openapi.md
- name: AWS EC2 API - Import Snapshot
  x-api-slug: actionimportsnapshot-get
  description: Describes your import snapshot tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Compute_AmazonEC2.png
  humanURL: https://aws.amazon.com/ec2/
  baseURL: :///
  tags: Amazon Web Services, Compute, Stack Network, Stack, API Service Provider,
    API Service Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionimportsnapshot-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-ec2/actionimportsnapshot-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.dynamodb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.ec2.stack.network
- type: x-code
  url: http://aws.amazon.com/code/Amazon-EC2/
- type: x-documentation
  url: http://docs.aws.amazon.com/AWSEC2/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/ec2/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/ec2/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/ec2/pricing/
- type: x-sla
  url: https://aws.amazon.com/ec2/sla/
- type: x-website
  url: https://aws.amazon.com/ec2/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---