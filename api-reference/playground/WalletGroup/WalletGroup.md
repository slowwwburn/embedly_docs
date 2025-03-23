# Get All Wallet Groups

The `GET /api/v1/walletgroups/get` endpoint retrieves a list of all wallet groups.

## Request

### **URL**

`https://api/v1/walletgroups/get`

## Response

✅ Success Response

```json
Status Code: 200 OK

{
  "code": "00",
  "success": true,
  "message": "Retrieved Successfully",
  "data": [
    {
      "id": "d1d0e7a1-0830-11f0-a8a9-6045bd97b81d",
      "name": "string",
      "walletGroupFeatureDto": []
    },
    {
      "id": "dc56bc91-0833-11f0-a8a9-6045bd97b81d",
      "name": "Idbanc",
      "walletGroupFeatureDto": []
    }
  ]
}

```

## ❌ Error Responses

```json

Status Code: 500 Internal Server Error

{
  "code": "500",
  "success": false,
  "message": "An unexpected error occurred",
  "data": null
}
