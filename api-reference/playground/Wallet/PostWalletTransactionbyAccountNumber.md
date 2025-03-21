# Post Wallet Transaction by Account Number API

The `PUT /api/v1/wallets/wallet/transaction/account-number/post` endpoint posts a transaction to a specified wallet using the account number.

### **Request Method**

`PUT`

### **Request Body**

```json
{
  "id": 0,
  "productId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "organizationId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "amount": 0,
  "fee": 0,
  "postedDate": "2025-03-20T18:28:13.015Z",
  "valueDate": "2025-03-20T18:28:13.015Z",
  "transactionReference": "string",
  "walletId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "customerId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "isPosted": true,
  "direction": "string",
  "remarks": "string",
  "currency": "string",
  "batchReference": "string",
  "accountNumber": "string"
}
```

## Sample Response

✅ Success Response

```json
Status Code: 200 OK

{
  "code": "200",
  "success": true,
  "message": "Transaction posted successfully.",
  "data": {
    // Additional data fields if applicable
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

Status Code: 404 Not Found

{
  "code": "404",
  "success": false,
  "message": "Invalid account number and organization",
  "data": null
}

Status Code: 401 Unauthorized

{
  "code": "401",
  "success": false,
  "message": "Unauthorized access",
  "data": null
}

Status Code: 500 Internal Server Error

{
  "code": "500",
  "success": false,
  "message": "An unexpected error occurred",
  "data": null
}

```
