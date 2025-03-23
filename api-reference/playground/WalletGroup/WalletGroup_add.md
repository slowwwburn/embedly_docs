# Add Wallet Group

The `POST /api/v1/walletgroups/add` endpoint allows you to create a new wallet group.

## Request

### **URL**

`https://api/v1/walletgroups/add`

### **Request Body**

```json
{
  "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "name": "string",
  "walletGroupFeatureDto": [
    {
      "featureName": "string",
      "featurePropertyName": "string",
      "featurePropertyValue": "string"
    }
  ]
}
```

## Response

✅ Success Response

```json
Status Code: 200 Ok
{
  "code": "00",
  "success": true,
  "message": "Created Successfully",
  "data": {
    "id": "d1d0e7a1-0830-11f0-a8a9-6045bd97b81d",
    "name": "string",
    "walletGroupFeatureDto": null
  }
}

```

## ❌ Error Responses

```json
Status Code: 400 Bad Request
{
  "code": "400",
  "success": false,
  "message": "Invalid request data",
  "data": null
}

Status Code: 500 Internal Server Error

{
  "code": "500",
  "success": false,
  "message": "An unexpected error occurred",
  "data": null
}
