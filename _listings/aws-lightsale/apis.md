---
name: AWS Lightsale
x-slug: aws-lightsale
description: Amazon Lightsail is the easiest way to get started with AWS for developers
  who just need virtual private servers. Lightsail includes everything you need to
  launch your project quickly - a virtual machine, SSD-based storage, data transfer,
  DNS management, and a static IP - for a low, predictable price. You manage those
  Lightsail servers through the Lightsail console or by using the API or command-line
  interface (CLI).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Snapshots
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Lightsale API - Get Instance Snapshots
  x-api-slug: actiongetinstancesnapshots-get
  description: Returns all instance snapshots for the user's account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/actiongetinstancesnapshots-get-openapi.md
- name: AWS Lightsale API - Create Instances From Snapshot
  x-api-slug: actioncreateinstancesfromsnapshot-get
  description: |-
    Uses a specific snapshot as a blueprint for creating one or more new instances that are
          based on that identical configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/actioncreateinstancesfromsnapshot-get-openapi.md
- name: AWS Lightsale API - Create Instance Snapshot
  x-api-slug: actioncreateinstancesnapshot-get
  description: |-
    Creates a snapshot of a specific virtual private server, or
            instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/actioncreateinstancesnapshot-get-openapi.md
- name: AWS Lightsale API - Delete Instance Snapshot
  x-api-slug: actiondeleteinstancesnapshot-get
  description: |-
    Deletes a specific snapshot of a virtual private server (or
            instance).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/actiondeleteinstancesnapshot-get-openapi.md
- name: AWS Lightsale API - Get Instance Snapshot
  x-api-slug: actiongetinstancesnapshot-get
  description: Returns information about a specific instance snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/actiongetinstancesnapshot-get-openapi.md
- name: AWS Lightsale API - Get Instance Snapshots
  x-api-slug: actiongetinstancesnapshots-get
  description: Returns all instance snapshots for the user's account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Amazon Web Services, DNS, Stack Network, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-lightsale/actiongetinstancesnapshots-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.lambda.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.lightsale.stack.network
- type: x-documentation
  url: https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/Welcome.html?fid=6DDA37DF97F08F8B-23761D4A79F7B1E
- type: x-pricing
  url: https://amazonlightsail.com/pricing/
- type: x-website
  url: https://amazonlightsail.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---