{
  "info": {
    "name": "Microsoft Graph API Get Chart Data Labels",
    "_postman_id": "329ebc52-e632-4c7f-a673-14df86c18065",
    "description": "Get ChartDataLabels Retrieve the properties and relationships of chartdatalabels object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "chart",
      "item": [
        {
          "id": "43fe64ec-7378-4628-a427-68762436086d",
          "name": "GetChartDataLabels",
          "request": {
            "url": "http://graph.microsoft.com/, Data, Labels",
            "method": "GET",
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
            "description": "Get ChartDataLabels Retrieve the properties and relationships of chartdatalabels object"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "c47647d6-c7a5-48a1-809b-661d26276b72"
            }
          ]
        }
      ]
    }
  ]
}