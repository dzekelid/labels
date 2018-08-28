{
  "info": {
    "name": "Microsoft Graph API Update Chartdatalabels",
    "_postman_id": "09807a79-2c47-41c9-86bf-4d16e0e4bd3e",
    "description": "Update chartdatalabels Update the properties of chartdatalabels object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "chartdatalabels",
      "item": [
        {
          "id": "a0680fd2-2e5f-462b-a1e9-40f9377f30b6",
          "name": "UpdateChartdatalabels",
          "request": {
            "url": "http://graph.microsoft.com/datalabels",
            "method": "PATCH",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update chartdatalabels Update the properties of chartdatalabels object"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "ec1db2ef-6813-4fa1-8f15-6fda535d038f"
            }
          ]
        }
      ]
    }
  ]
}