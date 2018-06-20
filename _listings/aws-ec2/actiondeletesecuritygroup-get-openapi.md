---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Delete Security Group
  version: 1.0.0
  description: Deletes a security group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeSecurityGroupEgress (EC2-VPC only):
    get:
      summary: Authorize Security Group Egress ( E C2- V P C only)
      description: '[EC2-VPC only] Adds one or more egress rules to a security group
        for use with a VPC.'
      operationId: authorizesecuritygroupegress-ec2vpc-only
      x-api-path-slug: actionauthorizesecuritygroupegress-ec2vpc-only-get
      parameters:
      - in: query
        name: CidrIp
        description: The CIDR IPv4 address range
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: FromPort
        description: The start of port range for the TCP and UDP protocols, or an
          ICMP/ICMPv6 type number
        type: string
      - in: query
        name: GroupId
        description: The ID of the security group
        type: string
      - in: query
        name: GroupName
        description: '[EC2-Classic, default VPC] The name of the security group'
        type: string
      - in: query
        name: IpPermissions.N
        description: A set of IP permissions
        type: string
      - in: query
        name: IpProtocol
        description: The IP protocol name (tcp, udp, icmp) or number      (see Protocol
          Numbers)
        type: string
      - in: query
        name: SourceSecurityGroupName
        description: '[EC2-Classic, default VPC] The name of the source security group'
        type: string
      - in: query
        name: SourceSecurityGroupOwnerId
        description: '[EC2-Classic] The AWS account number for the source security
          group, if the source security group is in a different account'
        type: string
      - in: query
        name: ToPort
        description: The end of port range for the TCP and UDP protocols, or an ICMP/ICMPv6
          code number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Group
  /?Action=AuthorizeSecurityGroupIngress:
    get:
      summary: Authorize Security Group Ingress
      description: Adds one or more ingress rules to a security group.
      operationId: authorizesecuritygroupingress
      x-api-path-slug: actionauthorizesecuritygroupingress-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: GroupDescription
        description: A description for the security group
        type: string
      - in: query
        name: GroupName
        description: The name of the security group
        type: string
      - in: query
        name: VpcId
        description: '[EC2-VPC] The ID of the VPC'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Group
  /?Action=CreateSecurityGroup:
    get:
      summary: Create Security Group
      description: Creates a security group.
      operationId: createsecuritygroup
      x-api-path-slug: actioncreatesecuritygroup-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: GroupId
        description: The ID of the security group
        type: string
      - in: query
        name: GroupName
        description: '[EC2-Classic, default VPC] The name of the security group'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Group
  /?Action=DeleteSecurityGroup:
    get:
      summary: Delete Security Group
      description: Deletes a security group.
      operationId: deletesecuritygroup
      x-api-path-slug: actiondeletesecuritygroup-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the operation,
          without actually making the request, and provides an error response
        type: string
      - in: query
        name: GroupId.N
        description: One or more security group IDs in your account
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security  Group
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