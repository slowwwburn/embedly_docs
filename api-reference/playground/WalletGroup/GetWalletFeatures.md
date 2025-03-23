# Get Wallet Features API

The `GET /api/v1/walletgroups/walletfeatures/get` endpoint retrieves a list of available wallet features.

## Request

### **URL**

`https://api/v1/walletgroups/walletfeatures/get`

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
      "id": "025adebc-a8c9-432c-bbc1-45724b63aa63",
      "name": "Balance Limit",
      "description": "wallets with limit on balances",
      "direction": "C",
      "isPercentage": false,
      "isEveryMonth": false,
      "isEveryTransaction": true,
      "hasMinimumAmount": true,
      "hasMaximumAmount": true,
      "walletFeaturePropertyDtos": [
        {
          "name": "Limit Amount",
          "dataType": "decimal"
        }
      ]
    },
    {
      "id": "3c372c8a-ce4f-4c21-8958-08ee045b3be2",
      "name": "Service Charge",
      "description": "Monthly service charge",
      "direction": "D",
      "isPercentage": true,
      "isEveryMonth": true,
      "isEveryTransaction": false,
      "hasMinimumAmount": false,
      "hasMaximumAmount": false,
      "walletFeaturePropertyDtos": [
        {
          "name": "Amount",
          "dataType": "decimal"
        }
      ]
    },
    {
      "id": "48bf7431-8ead-4c55-87b4-271daa05bb7a",
      "name": "Stamp Duty",
      "description": "stamp duty payments",
      "direction": "D",
      "isPercentage": false,
      "isEveryMonth": false,
      "isEveryTransaction": true,
      "hasMinimumAmount": false,
      "hasMaximumAmount": false,
      "walletFeaturePropertyDtos": [
        {
          "name": "Amount",
          "dataType": "decimal"
        }
      ]
    },
    {
      "id": "5d2f3a44-6766-4250-8b1f-7cf30e77e438",
      "name": "Dormancy",
      "description": "Accounts that will automatically go into PND due to inactivity for some time",
      "direction": "D",
      "isPercentage": false,
      "isEveryMonth": true,
      "isEveryTransaction": false,
      "hasMinimumAmount": false,
      "hasMaximumAmount": false,
      "walletFeaturePropertyDtos": [
        {
          "name": "Number of Months",
          "dataType": "int"
        }
      ]
    },
    {
      "id": "d447bddf-1bcb-4394-9ba7-cc1faf653126",
      "name": "Interests",
      "description": "Interest yielding wallet",
      "direction": "C",
      "isPercentage": true,
      "isEveryMonth": true,
      "isEveryTransaction": false,
      "hasMinimumAmount": false,
      "hasMaximumAmount": false,
      "walletFeaturePropertyDtos": [
        {
          "name": "Interest Rate",
          "dataType": "decimal"
        },
        {
          "name": "Maximum Withdrawal",
          "dataType": "int"
        }
      ]
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
