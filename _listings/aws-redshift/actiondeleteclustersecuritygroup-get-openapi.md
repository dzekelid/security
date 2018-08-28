---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Delete Cluster Security Group
  version: 1.0.0
  description: Deletes an Amazon Redshift security group.
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
  /?Action=CreateHsmConfiguration:
    get:
      summary: Create Hsm Configuration
      description: |-
        Creates an HSM configuration that contains the information required by an Amazon Redshift
                    cluster to store and use database encryption keys in a Hardware Security Module (HSM).
      operationId: createHsmConfiguration
      x-api-path-slug: actioncreatehsmconfiguration-get
      parameters:
      - in: query
        name: Description
        description: A text description of the HSM configuration to be created
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier to be assigned to the new Amazon Redshift HSM
          configuration
        type: string
      - in: query
        name: HsmIpAddress
        description: The IP address that the Amazon Redshift cluster must use to access
          the HSM
        type: string
      - in: query
        name: HsmPartitionName
        description: The name of the partition in the HSM where the Amazon Redshift
          clusters will store their            database encryption keys
        type: string
      - in: query
        name: HsmPartitionPassword
        description: The password required to access the HSM partition
        type: string
      - in: query
        name: HsmServerPublicCertificate
        description: The HSMs public certificate file
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---