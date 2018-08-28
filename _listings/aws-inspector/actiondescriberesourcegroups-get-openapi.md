---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Describe Resource Groups
  version: 1.0.0
  description: |-
    Describes the resource groups that are specified by the ARNs of the resource
             groups.
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