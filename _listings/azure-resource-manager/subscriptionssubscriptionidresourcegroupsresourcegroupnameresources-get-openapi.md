---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 0
info:
  title: Azure Resource Manager API Resource Groups List Resources
  description: Get all the resources for a resource group.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/resources:
    get:
      summary: Resource Groups List Resources
      description: Get all the resources for a resource group.
      operationId: ResourceGroups_ListResources
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get
      parameters:
      - in: query
        name: $expand
        description: The $expand query parameter
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group with the resources to get
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