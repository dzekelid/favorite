{
  "info": {
    "name": "Dezrez Returns favorite regions",
    "_postman_id": "19b1e31e-c0ea-49f6-b70d-6fffd56b1cf7",
    "description": "Returns favorite regions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "255894fd-3bc3-4571-becd-f6bdd87bbfe2",
          "name": "Region_GetAllFavourites",
          "request": {
            "url": "http://api.dezrez.com/api/region/favourites",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns favorite regions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb8b7abc-7d87-4b3e-b7f1-0da82d16ad64"
            }
          ]
        }
      ]
    }
  ]
}