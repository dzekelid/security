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
tags: Security
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Redshift API Authorize Cluster Security Group Ingress
  x-api-slug: amazon-redshift-api
  description: Adds an inbound (ingress) rule to an Amazon Redshift security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=AuthorizeClusterSecurityGroupIngress
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/actionauthorizeclustersecuritygroupingress-get-openapi.md
- name: Amazon Redshift API Create Cluster Security Group
  x-api-slug: amazon-redshift-api
  description: Creates a new Amazon Redshift security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterSecurityGroup
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/actioncreateclustersecuritygroup-get-openapi.md
- name: Amazon Redshift API Delete Cluster Security Group
  x-api-slug: amazon-redshift-api
  description: Deletes an Amazon Redshift security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterSecurityGroup
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/actiondeleteclustersecuritygroup-get-openapi.md
- name: Amazon Redshift API Describe Cluster Security Groups
  x-api-slug: amazon-redshift-api
  description: Returns information about Amazon Redshift security groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterSecurityGroups
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/actiondescribeclustersecuritygroups-get-openapi.md
- name: Amazon Redshift API Revoke Cluster Security Group Ingress
  x-api-slug: amazon-redshift-api
  description: |-
    Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                IP range or Amazon EC2 security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RevokeClusterSecurityGroupIngress
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/actionrevokeclustersecuritygroupingress-get-openapi.md
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
  tags: Security
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/security/master/_listings/aws-redshift/openapi.md
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