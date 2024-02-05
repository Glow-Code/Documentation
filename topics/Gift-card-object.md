# Gift card object

The gift card object is the same format when returned from any endpoint that returns a gift card. The gift card object has the following structure:

```json
{
    "data": {
        "id": "9b3de229-fbe0-4e33-b5ac-cb3f6003d471",
        "value": {
            "amount": "1000",
            "currency": "GBP",
            "formatted": "£10.00"
        },
        "issue_fee": null,
        "type": "recipient_choice",
        "email_address": null,
        "mobile_number": null,
        "idempotency_key": "9af0e1ce-c130-4aac-83dc-4144d2b1591a-unique_key_22222",
        "created_at": "2024-02-02T19:08:17.000000Z",
        "updated_at": "2024-02-02T19:08:17.000000Z",
        "redemption_url": "https://url",
        "cards": []
    }
}
```

## Object properties

<table>
    <tr>
        <th>Field</th>
        <th>Type</th>
        <th>Description</th>
    </tr>
    <tr>
        <td>id</td>
        <td>string</td>
        <td>The unique identifier of the gift card.</td>
    </tr>
    <tr>
        <td>value</td>
        <td>object</td>
        <td>The value of the gift card.</td>
    </tr>
    <tr>
        <td>issue_fee</td>
        <td>object</td>
        <td>
The issue fee of the gift card.

> Not all gift cards have an issue fee.
</td>
    </tr>
    <tr>
        <td>type</td>
        <td>string</td>
        <td>
The type of the gift card.

> Possible values are `send` and `recipient_choice`.
</td>
    </tr>
    <tr>
        <td>email_address</td>
        <td>string</td>
        <td>The email address of the recipient of the gift card.</td>
    </tr>
    <tr>
        <td>mobile_number</td>
        <td>string</td>
        <td>The mobile number of the recipient of the gift card.</td>
    </tr>
    <tr>
        <td>idempotency_key</td>
        <td>string</td>
        <td>The idempotency key of the gift card.</td>
    </tr>
    <tr>
        <td>created_at</td>
        <td>string</td>
        <td>The date and time when the gift card was created.</td>
    </tr>
    <tr>
        <td>updated_at</td>
        <td>string</td>
        <td>The date and time when the gift card was last updated.</td>
    </tr>
    <tr>
        <td>redemption_url</td>
        <td>string</td>
        <td>The URL where the recipient can redeem the gift card.</td>
    </tr>
    <tr>
        <td>cards</td>
        <td>array</td>
        <td>An array of child gift cards associated with the gift card. This is the case when a gift card has been split into multiple gift cards.</td>
    </tr>
</table>
