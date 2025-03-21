# Restrict Wallet API

## Overview  

The `PATCH /api/v1/wallets/wallet/restrict` endpoint restricts a specified wallet by updating its details.

## Request

### **URL**

`https:///api/v1/wallets/wallet/restrict`

### **Request Method**

`PATCH`

### **Request Body**

```json
{
  "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "walletGroupId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "customerId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "availableBalance": 0,
  "ledgerBalance": 0,
  "walletRestrictionId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "walletClassificationId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "currencyId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  "isInternal": true,
  "isDefault": true,
  "name": "Victor Imah",
  "overdraft": 0,
  "virtualAccount": {
    "accountNumber": "30235699911",
    "bankCode": "040",
    "bankName": "Polaris Bank"
  },
  "mobNum": "09030355074",
  "customerTypeId": "3fa85f64-5717-4562-b3fc-2c963f66afa6"
}
```

## Response

✅ Success Response
Status Code: 200 OK

```json
{
  "code": "200",
  "success": true,
  "message": "Wallet restricted successfully.",
  "data": {
    "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
  }
}
```
