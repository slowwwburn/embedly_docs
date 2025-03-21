# Close Wallet by Account

The `GET /api/v1/wallets/can/close/account/{accountId}` endpoint checks if a specified wallet can be closed based on the account ID.

## Request

### **URL**

`https://api/v1/wallets/can/close/account/{accountId}`

### **Request Method**

`GET`

### **Path Parameters**

| Parameter    | Type   | Description                              |
|--------------|--------|------------------------------------------|
| `accountId`  | string | Unique identifier for the account (required). |

## Request URL

### Response

```json
✅ Success Response
Status Code: 200 OK
{
  "code": "200",
  "success": true,
  "message": "You can close this account.",
  "data": {
    // Additional details if applicable
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

Status Code: 401 Unauthorized

{
  "code": "401",
  "success": false,
  "message": "You do not have rights to access this account",
  "data": null
}

Status Code: 403 Forbidden

{
  "code": "403",
  "success": false,
  "message": "Access denied for this operation",
  "data": null
}

Status Code: 500 Internal Server Error

{
  "code": "500",
  "success": false,
  "message": "An unexpected error occurred",
  "data": null
}

