{
  "info": {
    "name": "Dezrez Returns favorite regions",
    "_postman_id": "499faea9-7a87-4614-aaa3-0ae2ea3c3d0e",
    "description": "Returns favorite regions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "7cf666c3-b889-4a5e-8d0c-fa80e3c73057",
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
              "id": "864b613d-a8ef-4181-9ff6-a7f004395b5d"
            }
          ]
        },
        {
          "id": "cd59f0f5-c1fb-4aa4-8a46-adf63d432dee",
          "name": "Region_GetFavouriteByfavouriteRegionId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/region/favourites/:favouriteRegionId"
              ],
              "variable": [
                {
                  "id": "favouriteRegionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
              "id": "0716ddd1-0513-4215-a448-c16bd9bcb52a"
            }
          ]
        }
      ]
    }
  ]
}