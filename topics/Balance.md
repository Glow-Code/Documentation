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
            "amount": "2000",
            "amount_decimal": "20.00",
            "formatted_amount": "£20.00",
            "updated_at": "2023-01-01 00:00:00"
        },
        {
            "currency": "USD",
            "amount": "2000",
            "amount_decimal": "20.00",
            "formatted_amount": "$20.00",
            "updated_at": "2023-01-01 00:00:00"
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
</table>
