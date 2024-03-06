# Balance

This endpoint allows you to check the balance of your account's wallet.

## Endpoint

```http
GET %url%balances
```

## Response

```json
{
  "data": [
    {
      "currency": "GBP",
      "amount": "-75000",
      "amount_decimal": "-750.00",
      "formatted_amount": "(£750.00)",
      "updated_at": "2024-03-06T21:49:02.000000Z",
      "limits": {
        "daily": {
          "limit": {
            "amount": "100000",
            "currency": "GBP",
            "formatted": "£1,000.00"
          },
          "remaining": {
            "amount": "25000",
            "currency": "GBP",
            "formatted": "£250.00"
          }
        },
        "monthly": {
          "limit": {
            "amount": "100000",
            "currency": "GBP",
            "formatted": "£1,000.00"
          },
          "remaining": {
            "amount": "25000",
            "currency": "GBP",
            "formatted": "£250.00"
          }
        }
      }
    },
    {
      "currency": "USD",
      "amount": "0",
      "amount_decimal": "0.00",
      "formatted_amount": "$0.00",
      "updated_at": "2024-03-05T21:58:08.000000Z",
      "limits": {
        "daily": {
          "limit": {
            "amount": "100000",
            "currency": "USD",
            "formatted": "$1,000.00"
          },
          "remaining": {
            "amount": "25000",
            "currency": "USD",
            "formatted": "$250.00"
          }
        },
        "monthly": {
          "limit": {
            "amount": "100000",
            "currency": "USD",
            "formatted": "$1,000.00"
          },
          "remaining": {
            "amount": "25000",
            "currency": "USD",
            "formatted": "$250.00"
          }
        }
      }
    }
  ]
}
```

<table>
    <tr>
        <th>Field</th>
        <th>Type</th>
        <th>Description</th>
    </tr>
    <tr>
        <td>currency</td>
        <td>string</td>
        <td>The currency of the balance</td>
    </tr>
    <tr>
        <td>amount</td>
        <td>string</td>
        <td>The amount of the balance in the currencies smallest unit</td>
    </tr>
    <tr>
        <td>amount_decimal</td>
        <td>string</td>
        <td>The amount of the balance as a decimal</td>
    </tr>
    <tr>
        <td>formatted_amount</td>
        <td>string</td>
        <td>The amount of the balance formatted as a string with symbol</td>
    </tr>
    <tr>
        <td>updated_at</td>
        <td>object</td>
        <td>The date and time the balance was last updated</td>
    </tr>
    <tr>
        <td>limits</td>
        <td>object</td>
        <td>Accounts are protected from excessive spending by account limits, the limit object contains the limit and remaining limit allowance.</td>
    </tr>
</table>
