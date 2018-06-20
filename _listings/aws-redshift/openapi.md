---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeClusterSecurityGroupIngress:
    get:
      summary: Authorize Cluster Security Group Ingress
      description: Adds an inbound (ingress) rule to an Amazon Redshift security group.
      operationId: authorizeClusterSecurityGroupIngress
      x-api-path-slug: actionauthorizeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to be added the Amazon Redshift security group
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security group to which the ingress rule is added
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The EC2 security group to be added the Amazon Redshift security
          group
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          by the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=CreateClusterSecurityGroup:
    get:
      summary: Create Cluster Security Group
      description: Creates a new Amazon Redshift security group.
      operationId: createClusterSecurityGroup
      x-api-path-slug: actioncreateclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name for the security group
        type: string
      - in: query
        name: Description
        description: A description for the security group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DeleteClusterSecurityGroup:
    get:
      summary: Delete Cluster Security Group
      description: Deletes an Amazon Redshift security group.
      operationId: deleteClusterSecurityGroup
      x-api-path-slug: actiondeleteclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the cluster security group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DescribeClusterSecurityGroups:
    get:
      summary: Describe Cluster Security Groups
      description: Returns information about Amazon Redshift security groups.
      operationId: describeClusterSecurityGroups
      x-api-path-slug: actiondescribeclustersecuritygroups-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of a cluster security group for which you are requesting
          details
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          security groups            that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster security            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=RevokeClusterSecurityGroupIngress:
    get:
      summary: Revoke Cluster Security Group Ingress
      description: |-
        Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                    IP range or Amazon EC2 security group.
      operationId: revokeClusterSecurityGroupIngress
      x-api-path-slug: actionrevokeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range for which to revoke access
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security Group from which to revoke the ingress
          rule
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the EC2 Security Group whose access is to be revoked
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          in the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
---