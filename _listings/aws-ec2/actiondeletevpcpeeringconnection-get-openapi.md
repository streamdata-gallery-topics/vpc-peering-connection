---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Delete Vpc Peering Connection
  version: 1.0.0
  description: Deletes a VPC peering connection.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptVpcPeeringConnection:
    get:
      summary: Accept Vpc Peering Connection
      description: Accept a VPC peering connection request.
      operationId: acceptvpcpeeringconnection
      x-api-path-slug: actionacceptvpcpeeringconnection-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: PeerOwnerId
        description: The AWS account ID of the owner of the peer VPC
        type: string
      - in: query
        name: PeerVpcId
        description: The ID of the VPC with which you are creating the VPC peering
          connection
        type: string
      - in: query
        name: VpcId
        description: The ID of the requester VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Peering Connection
  /?Action=CreateVpcPeeringConnection:
    get:
      summary: Create Vpc Peering Connection
      description: 'Requests a VPC peering connection between two VPCs: a requester
        VPC that you own and a peer VPC with which to create the connection.'
      operationId: createvpcpeeringconnection
      x-api-path-slug: actioncreatevpcpeeringconnection-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: VpcPeeringConnectionId
        description: The ID of the VPC peering connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Peering Connection
  /?Action=DeleteVpcPeeringConnection:
    get:
      summary: Delete Vpc Peering Connection
      description: Deletes a VPC peering connection.
      operationId: deletevpcpeeringconnection
      x-api-path-slug: actiondeletevpcpeeringconnection-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: VpcPeeringConnectionId.N
        description: One or more VPC peering connection IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Peering Connection
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