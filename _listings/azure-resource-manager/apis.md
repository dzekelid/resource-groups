---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Resource Groups
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: SubscriptionClient - Resource Groups List Resources
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get
  description: Get all the resources for a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get-openapi.md
- name: SubscriptionClient - Resource Groups Get
  x-api-slug: subscriptionssubscriptionidresourcegroupsresourcegroupname-get
  description: Gets a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-get-openapi.md
- name: SubscriptionClient - Resource Groups List
  x-api-slug: subscriptionssubscriptionidresourcegroups-get
  description: Gets all the resource groups for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Microsoft, Resources, Links, API Service Provider, API Provider, Deployments,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/resource-groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroups-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://azure.resource.health.api.gallery.streamdata.io
- type: x-api-stack
  url: http://azure.resource.manager.stack.network
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---