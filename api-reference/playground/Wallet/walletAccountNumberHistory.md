# Account Number History API

## Overview  

The `POST /api/v1/wallets/account-number/history` endpoint retrieves the transaction history for a specific account number over a specified time range.

## Request

### **URL**

`/api/v1/wallets/account-number/history`

### **Request Method**

`POST`

### **Request Body**

```json
{
  "accountNumber": "211651123",
  "from": "2025-03-19T17:11:52.488Z",
  "to": "2025-03-19T17:11:52.488Z"
}


Response

❌ Error Responses
Status Code: 404 Not Found

{
  "code": "404",
  "success": false,
  "message": "Wallet not found",
  "data": null
}
