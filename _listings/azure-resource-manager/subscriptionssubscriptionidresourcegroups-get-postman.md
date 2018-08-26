{
  "info": {
    "name": "Azure Resource Manager API Resource Groups List",
    "_postman_id": "25ce1ccf-6cdc-4215-b7d9-cbd99f1f2d28",
    "description": "Gets all the resource groups for a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resource groups",
      "item": [
        {
          "id": "636d2c98-b5f5-4152-ad4b-8e94f2e643b0",
          "name": "ResourceGroups_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$top",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the resource groups for a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "967cd18f-052c-4289-80d0-58a6d908c6c1"
            }
          ]
        }
      ]
    }
  ]
}