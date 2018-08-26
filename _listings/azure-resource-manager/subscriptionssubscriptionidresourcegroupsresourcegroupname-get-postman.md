{
  "info": {
    "name": "Azure Resource Manager API Resource Groups Get",
    "_postman_id": "eda25eae-854f-406b-a1f3-dc3531eb6883",
    "description": "Gets a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "resource groups",
      "item": [
        {
          "id": "ec94a04a-10a7-4126-a90c-fd6aa85fbb3b",
          "name": "ResourceGroups_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourcegroups/:resourceGroupName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Gets a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9dc5306-76b5-4c6e-b04f-25d6876668ce"
            }
          ]
        }
      ]
    }
  ]
}