{
  "info": {
    "name": "Data.gov API Get Reuses Types",
    "_postman_id": "3e9ce49a-8007-404c-8373-4571d9c0d0ad",
    "description": "List all reuse types",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "reuses",
      "item": [
        {
          "id": "c032fb13-d8b7-4837-bbe7-46c707722157",
          "name": "getReusesTypes",
          "request": {
            "url": "http://catalog.data.gov/api/3/reuses/types/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all reuse types"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89e71593-5b47-45c5-9e5e-ef684097762f"
            }
          ]
        }
      ]
    }
  ]
}