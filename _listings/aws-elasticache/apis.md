---
name: AWS ElastiCache
x-slug: aws-elasticache
description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
  and scale an in-memory data store or cache in the cloud. The service improves the
  performance of web applications by allowing you to retrieve information from fast,
  managed, in-memory data stores, instead of relying entirely on slower disk-based
  databases. Amazon ElastiCache automatically detects and replaces failed nodes, reducing
  the overhead associated with self-managed infrastructures and provides a resilient
  system that mitigates the risk of overloaded databases, which slow website and application
  load times. Through integration with Amazon CloudWatch, Amazon ElastiCache provides
  enhanced visibility into key performance metrics associated with your Redis or Memcached
  nodes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Snapshots
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-elasticache/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon ElastiCache API Copy Snapshot
  x-api-slug: amazon-elasticache-api
  description: Makes a copy of an existing snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=CopySnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-elasticache/actioncopysnapshot-get-openapi.md
- name: Amazon ElastiCache API Create Snapshot
  x-api-slug: amazon-elasticache-api
  description: |-
    Creates a copy of an entire cache cluster or replication group at a
                specific moment in time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=CreateSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-elasticache/actioncreatesnapshot-get-openapi.md
- name: Amazon ElastiCache API Delete Snapshot
  x-api-slug: amazon-elasticache-api
  description: Deletes an existing snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DeleteSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-elasticache/actiondeletesnapshot-get-openapi.md
- name: Amazon ElastiCache API Describe Snapshots
  x-api-slug: amazon-elasticache-api
  description: Returns information about cache cluster or replication group snapshots.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DescribeSnapshots
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-elasticache/actiondescribesnapshots-get-openapi.md
- name: Amazon ElastiCache API
  x-api-slug: amazon-elasticache-api
  description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
    and scale an in-memory data store or cache in the cloud. The service improves
    the performance of web applications by allowing you to retrieve information from
    fast, managed, in-memory data stores, instead of relying entirely on slower disk-based
    databases. Amazon ElastiCache automatically detects and replaces failed nodes,
    reducing the overhead associated with self-managed infrastructures and provides
    a resilient system that mitigates the risk of overloaded databases, which slow
    website and application load times. Through integration with Amazon CloudWatch,
    Amazon ElastiCache provides enhanced visibility into key performance metrics associated
    with your Redis or Memcached nodes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-elasticache/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonElastiCache/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/elasticache/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticache/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticache/pricing/
- type: x-resources
  url: https://aws.amazon.com/elasticache/developer-resources/
- type: x-testimonials
  url: https://aws.amazon.com/elasticache/testimonials/
- type: x-website
  url: https://aws.amazon.com/elasticache/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---