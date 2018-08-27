swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateSubnetCidrBlock:
    get:
      summary: Associate Subnet Cidr Block
      description: Associates a CIDR block with your subnet.
      operationId: associatesubnetcidrblock
      x-api-path-slug: actionassociatesubnetcidrblock-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone for the subnet
        type: string
      - in: query
        name: CidrBlock
        description: The IPv4 network range for the subnet, in CIDR notation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Ipv6CidrBlock
        description: The IPv6 network range for the subnet, in CIDR notation
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
  /?Action=AssociateVpcCidrBlock:
    get:
      summary: Associate Vpc Cidr Block
      description: Associates a CIDR block with your VPC.
      operationId: associatevpccidrblock
      x-api-path-slug: actionassociatevpccidrblock-get
      parameters:
      - in: query
        name: AmazonProvidedIpv6CidrBlock
        description: Requests an Amazon-provided IPv6 CIDR block with a /56 prefix
          length for the VPC
        type: string
      - in: query
        name: CidrBlock
        description: The IPv4 network range for the VPC, in CIDR notation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceTenancy
        description: The tenancy options for instances launched into the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
  /?Action=DisassociateSubnetCidrBlock:
    get:
      summary: Disassociate Subnet Cidr Block
      description: Disassociates a CIDR block from a subnet.
      operationId: disassociatesubnetcidrblock
      x-api-path-slug: actiondisassociatesubnetcidrblock-get
      parameters:
      - in: query
        name: AssignIpv6AddressOnCreation
        description: Specify true to indicate that network interfaces created in the            specified
          subnet should be assigned an IPv6 address
        type: string
      - in: query
        name: MapPublicIpOnLaunch
        description: Specify true to indicate that network interfaces created in the            specified
          subnet should be assigned a public IPv4 address
        type: string
      - in: query
        name: SubnetId
        description: The ID of the subnet
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block
  /?Action=DisassociateVpcCidrBlock:
    get:
      summary: Disassociate Vpc Cidr Block
      description: Disassociates a CIDR block from a VPC.
      operationId: disassociatevpccidrblock
      x-api-path-slug: actiondisassociatevpccidrblock-get
      parameters:
      - in: query
        name: EnableDnsHostnames
        description: Indicates whether the instances launched in the VPC get DNS hostnames
        type: string
      - in: query
        name: EnableDnsSupport
        description: Indicates whether the DNS resolution is supported for the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - CIDR Block