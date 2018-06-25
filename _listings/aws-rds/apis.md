---
name: AWS RDS
x-slug: aws-rds
description: Amazon Relational Database Service (Amazon RDS) makes it easy to set
  up, operate, and scale arelational databasein the cloud. It provides cost-efficient
  and resizable capacity while managing time-consuming database administration tasks,
  freeing you up to focus on your applications and business. Amazon RDS provides you
  six familiar database engines to choose from, includingAmazon Aurora,PostgreSQL,MySQL,MariaDB,Oracle,
  andMicrosoft SQL Server.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Snapshots
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon RDS API Copy D B Cluster Snapshot
  x-api-slug: amazon-rds-api
  description: Creates a snapshot of a DB cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=CopyDBClusterSnapshot
  tags: Cluster Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actioncopydbclustersnapshot-get-openapi.md
- name: Amazon RDS API Copy D B Snapshot
  x-api-slug: amazon-rds-api
  description: Copies the specified DB snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=CopyDBSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actioncopydbsnapshot-get-openapi.md
- name: Amazon RDS API Create D B Cluster Snapshot
  x-api-slug: amazon-rds-api
  description: Creates a snapshot of a DB cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=CreateDBClusterSnapshot
  tags: Cluster Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actioncreatedbclustersnapshot-get-openapi.md
- name: Amazon RDS API Create D B Snapshot
  x-api-slug: amazon-rds-api
  description: Creates a DBSnapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=CreateDBSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actioncreatedbsnapshot-get-openapi.md
- name: Amazon RDS API Delete D B Cluster Snapshot
  x-api-slug: amazon-rds-api
  description: Deletes a DB cluster snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DeleteDBClusterSnapshot
  tags: Cluster Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actiondeletedbclustersnapshot-get-openapi.md
- name: Amazon RDS API Delete D B Snapshot
  x-api-slug: amazon-rds-api
  description: Deletes a DBSnapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DeleteDBSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actiondeletedbsnapshot-get-openapi.md
- name: Amazon RDS API Describe D B Cluster Snapshot Attributes
  x-api-slug: amazon-rds-api
  description: Returns a list of DB cluster snapshot attribute names and values for
    a manual DB cluster snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeDBClusterSnapshotAttributes
  tags: Cluster Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actiondescribedbclustersnapshotattributes-get-openapi.md
- name: Amazon RDS API Describe D B Cluster Snapshots
  x-api-slug: amazon-rds-api
  description: Returns information about DB cluster snapshots.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeDBClusterSnapshots
  tags: Cluster Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actiondescribedbclustersnapshots-get-openapi.md
- name: Amazon RDS API Describe D B Snapshot Attributes
  x-api-slug: amazon-rds-api
  description: Returns a list of DB snapshot attribute names and values for a manual
    DB snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeDBSnapshotAttributes
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actiondescribedbsnapshotattributes-get-openapi.md
- name: Amazon RDS API Describe D B Snapshots
  x-api-slug: amazon-rds-api
  description: Returns information about DB snapshots.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeDBSnapshots
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actiondescribedbsnapshots-get-openapi.md
- name: Amazon RDS API Modify D B Cluster Snapshot Attribute
  x-api-slug: amazon-rds-api
  description: Adds an attribute and values to, or removes an attribute and values
    from, a manual DB cluster snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=ModifyDBClusterSnapshotAttribute
  tags: Cluster Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actionmodifydbclustersnapshotattribute-get-openapi.md
- name: Amazon RDS API Modify D B Snapshot Attribute
  x-api-slug: amazon-rds-api
  description: Adds an attribute and values to, or removes an attribute and values
    from, a manual DB snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=ModifyDBSnapshotAttribute
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actionmodifydbsnapshotattribute-get-openapi.md
- name: Amazon RDS API Restore D B Cluster From Snapshot
  x-api-slug: amazon-rds-api
  description: Creates a new DB cluster from a DB cluster snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=RestoreDBClusterFromSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/actionrestoredbclusterfromsnapshot-get-openapi.md
- name: Amazon RDS API
  x-api-slug: amazon-rds-api
  description: Amazon Relational Database Service (Amazon RDS) makes it easy to set
    up, operate, and scale arelational databasein the cloud. It provides cost-efficient
    and resizable capacity while managing time-consuming database administration tasks,
    freeing you up to focus on your applications and business. Amazon RDS provides
    you six familiar database engines to choose from, includingAmazon Aurora,PostgreSQL,MySQL,MariaDB,Oracle,
    andMicrosoft SQL Server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: :///
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-rds/openapi.md
x-common:
- type: x-articles
  url: https://aws.amazon.com/articles/Amazon-RDS
- type: x-blog
  url: https://aws.amazon.com/blogs/database/
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=291
- type: x-code
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=293
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/AmazonRDS/latest/CommandLineReference/
- type: x-customer-highlights
  url: https://aws.amazon.com/rds/customers/
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonRDS/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/rds/faqs/
- type: x-forum
  url: http://developer.amazonwebservices.com/connect/forum.jspa?forumID=60
- type: x-getting-started
  url: https://aws.amazon.com/rds/getting-started/
- type: x-partners
  url: https://aws.amazon.com/rds/partners/
- type: x-pricing
  url: https://aws.amazon.com/rds/pricing/
- type: x-service-level-agreement
  url: https://aws.amazon.com/rds/sla/
- type: x-tools
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=294
- type: x-website
  url: https://aws.amazon.com/rds/
- type: x-whats-new
  url: https://aws.amazon.com/rds/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---