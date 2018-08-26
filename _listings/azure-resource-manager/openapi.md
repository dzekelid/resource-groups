---
swagger: "2.0"
x-collection-name: Azure Resource Manager
x-complete: 1
info:
  title: SubscriptionClient
  description: all-resource-groups-and-resources-exist-within-subscriptions--these-operation-enable-you-get-information-about-your-subscriptions-and-tenants--a-tenant-is-a-dedicated-instance-of-azure-active-directory-azure-ad-for-your-organization-
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
  /subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}:
    put:
      summary: Resource Groups Create Or Update
      description: Creates a resource group.
      operationId: ResourceGroups_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the create or update a resource group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group to create or update
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
    get:
      summary: Resource Groups Get
      description: Gets a resource group.
      operationId: ResourceGroups_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group to get
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
  /subscriptions/{subscriptionId}/resourcegroups:
    get:
      summary: Resource Groups List
      description: Gets all the resource groups for a subscription.
      operationId: ResourceGroups_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroups-get
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: The number of results to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Resource Groups
---