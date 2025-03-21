# Get Customer Wallet API

## Overview  

The `GET /api/v1/wallets/get/customer/{customerId}/wallet/{walletId}` endpoint retrieves the details of a specific wallet associated with a customer.

## Request

### **URL**

`/api/v1/wallets/get/customer/{customerId}/wallet/{walletId}`

### **Request Method**

`GET`

### **Path Parameters**

| Parameter     | Type   | Description                              |
|---------------|--------|------------------------------------------|
| `customerId`  | string | Unique identifier for the customer (required). |
| `walletId`    | string | Unique identifier for the wallet (required).   |

## Response

### ✅ Success Response

- **Status Code**: `200 OK`

```json
{
  "code": "200",
  "success": true,
  "message": "Wallet details retrieved successfully.",
  "data": {
    "walletId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
    "customerId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
    "availableBalance": 10000,
    "ledgerBalance": 12000,
    "currency": "USD",
    "status": "active"
  }
}
```

### ❌ Error Responses

Status Code: 400 Bad Request

```json
{
  "code": "400",
  "success": false,
  "message": "Invalid customer ID specified",
  "data": null
}
```
