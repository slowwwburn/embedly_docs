# Get Wallet Group

The `GET /api/v1/walletgroups/get/{id}` endpoint retrieves details of a specified wallet group using its ID.

## Request

### **URL**

`https://api/v1/walletgroups/get/{id}`

### **Path Parameter**

| Parameter | Type   | Description                               |
|-----------|--------|-------------------------------------------|
| `id`      | string | The ID of the wallet group to retrieve (required). |

## Response

✅ Success Response

```json
Status Code: 200 OK

{
  "code": "00",
  "success": true,
  "message": "Wallet group retrieved successfully.",
  "data": {
    // Wallet group details here
  }
}
```

## ❌ Error Responses

```json

Status Code: 400 Bad Request

{
  "code": "400",
  "success": false,
  "message": "Invalid Wallet Group ID specified",
  "data": null
}

Status Code: 404 Not Found

{
  "code": "404",
  "success": false,
  "message": "Wallet group not found",
  "data": null
}

Status Code: 500 Internal Server Error

{
  "code": "500",
  "success": false,
  "message": "An unexpected error occurred",
  "data": null
}
