---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateResourceGroup:
    get:
      summary: Create Resource Group
      description: |-
        Creates a resource group using the specified set of tags (key and value pairs) that
                 are used to select the EC2 instances to be included in an Amazon Inspector assessment
                 target.
      operationId: createResourceGroup
      x-api-path-slug: actioncreateresourcegroup-get
      parameters:
      - in: query
        name: resourceGroupTags
        description: A collection of keys and an array of possible values,         [{key:key1,values:[Value1,Value2]},{key:Key2,values:[Value3]}]
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
  /?Action=DescribeResourceGroups:
    get:
      summary: Describe Resource Groups
      description: |-
        Describes the resource groups that are specified by the ARNs of the resource
                 groups.
      operationId: describeResourceGroups
      x-api-path-slug: actiondescriberesourcegroups-get
      parameters:
      - in: query
        name: resourceGroupArns
        description: The ARN that specifies the resource group that you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
---