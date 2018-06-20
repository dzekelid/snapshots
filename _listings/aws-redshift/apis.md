---
name: AWS Redshift
x-slug: aws-redshift
description: Amazon Redshift is a fast, fully managed, petabyte-scaledata warehousethat
  makes it simple and cost-effective to analyze all your data using your existing
  business intelligence tools. Start small for $0.25 per hour with no commitments
  and scale to petabytes for $1,000 per terabyte per year, less than a tenth the cost
  of traditional solutions. Customers typically see 3x compression, reducing their
  costs to $333 per uncompressed terabyte per year.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Snapshots
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Redshift API Authorize Snapshot Access
  x-api-slug: amazon-redshift-api
  description: |-
    Authorizes the specified AWS customer account to restore the specified
                snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=AuthorizeSnapshotAccess
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actionauthorizesnapshotaccess-get-openapi.md
- name: Amazon Redshift API Copy Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Copies the specified automated cluster snapshot to a new manual cluster
    snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CopyClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actioncopyclustersnapshot-get-openapi.md
- name: Amazon Redshift API Create Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Creates a manual snapshot of the specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actioncreateclustersnapshot-get-openapi.md
- name: Amazon Redshift API Create Snapshot Copy Grant
  x-api-slug: amazon-redshift-api
  description: |-
    Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                destination region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateSnapshotCopyGrant
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actioncreatesnapshotcopygrant-get-openapi.md
- name: Amazon Redshift API Delete Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Deletes the specified manual snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actiondeleteclustersnapshot-get-openapi.md
- name: Amazon Redshift API Delete Snapshot Copy Grant
  x-api-slug: amazon-redshift-api
  description: Deletes the specified snapshot copy grant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteSnapshotCopyGrant
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actiondeletesnapshotcopygrant-get-openapi.md
- name: Amazon Redshift API Describe Cluster Snapshots
  x-api-slug: amazon-redshift-api
  description: |-
    Returns one or more snapshot objects, which contain metadata about your cluster
                snapshots.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterSnapshots
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actiondescribeclustersnapshots-get-openapi.md
- name: Amazon Redshift API Describe Snapshot Copy Grants
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a list of snapshot copy grants owned by the AWS account in the destination
                region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeSnapshotCopyGrants
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actiondescribesnapshotcopygrants-get-openapi.md
- name: Amazon Redshift API Disable Snapshot Copy
  x-api-slug: amazon-redshift-api
  description: |-
    Disables the automatic copying of snapshots from one region to another region for a
                specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DisableSnapshotCopy
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actiondisablesnapshotcopy-get-openapi.md
- name: Amazon Redshift API Enable Snapshot Copy
  x-api-slug: amazon-redshift-api
  description: |-
    Enables the automatic copy of snapshots from one region to another region for a
                specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=EnableSnapshotCopy
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actionenablesnapshotcopy-get-openapi.md
- name: Amazon Redshift API Modify Snapshot Copy Retention Period
  x-api-slug: amazon-redshift-api
  description: |-
    Modifies the number of days to retain automated snapshots in the destination region
                after they are copied from the source region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifySnapshotCopyRetentionPeriod
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actionmodifysnapshotcopyretentionperiod-get-openapi.md
- name: Amazon Redshift API Restore From Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Creates a new cluster from a snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RestoreFromClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actionrestorefromclustersnapshot-get-openapi.md
- name: Amazon Redshift API Restore Table From Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Creates a new table from a table in an Amazon Redshift cluster snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RestoreTableFromClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actionrestoretablefromclustersnapshot-get-openapi.md
- name: Amazon Redshift API Revoke Snapshot Access
  x-api-slug: amazon-redshift-api
  description: |-
    Removes the ability of the specified AWS customer account to restore the specified
                snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RevokeSnapshotAccess
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/actionrevokesnapshotaccess-get-openapi.md
- name: Amazon Redshift API
  x-api-slug: amazon-redshift-api
  description: Amazon Redshift is a fast, fully managed, petabyte-scaledata warehousethat
    makes it simple and cost-effective to analyze all your data using your existing
    business intelligence tools. Start small for $0.25 per hour with no commitments
    and scale to petabytes for $1,000 per terabyte per year, less than a tenth the
    cost of traditional solutions. Customers typically see 3x compression, reducing
    their costs to $333 per uncompressed terabyte per year.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: :///
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/snapshots/master/_listings/aws-redshift/openapi.md
x-common:
- type: x-best-practices
  url: https://aws.amazon.com/redshift/developer-resources/#best-practices
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/redshift/index.html
- type: x-customer-success
  url: https://aws.amazon.com/redshift/customer-success/
- type: x-documentation
  url: http://docs.aws.amazon.com/redshift/latest/APIReference/
- type: x-events
  url: https://aws.amazon.com/redshift/events/
- type: x-faq
  url: https://aws.amazon.com/redshift/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/redshift/getting-started/
- type: x-partners
  url: https://aws.amazon.com/redshift/partners/
- type: x-pricing
  url: https://aws.amazon.com/redshift/pricing/
- type: x-website
  url: https://aws.amazon.com/redshift/
- type: x-whats-new
  url: https://aws.amazon.com/redshift/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---