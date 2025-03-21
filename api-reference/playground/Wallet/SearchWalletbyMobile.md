# Search Wallet by Mobile

The `GET /api/v1/wallets/search/mobile` endpoint allows you to search for a wallet associated with a specified mobile number.

---

## Request

### **URL**

`https://api/v1/wallets/search/mobile`

### **Query Parameters**

| Parameter     | Type   | Description                               |
|---------------|--------|-------------------------------------------|
| `mobile`      | string | Mobile number to search for (required).  |

## Response

✅ Success Response

```json
Status Code: 200 OK

{
  "code": "200",
  "success": true,
  "message": "Wallet found.",
  "data": {
    // Details of the wallet associated with the mobile number
  }
}

```

## ❌ Error Responses

``` json
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
  "message": "The key value at position 0 of the call to 'DbSet<VirtualAccountProvider>.Find' was of type 'int', which does not match the property type of 'Guid'.",
  "data": null
}
