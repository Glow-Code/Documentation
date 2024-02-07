# Purchase a gift card

> Please read the following documentation carefully to understand the different types of gift cards that available for
> purchase as well as the different delivery methods we support.
>
{style="warning"}

## Gift card types

There are two types of gift cards that can be purchased, a direct gift card and a recipient choice gift card.

{type="medium" sorted="desc"}
Direct gift card
: Direct gift cards are fixed to a specific brand and value.

Recipient choice gift {id="recipient-choice"}
: The recipient is able to split their gift card value across multiple brands. The sender defines the available brands
and the currency of the gift card by creating a template inside their account.

## Delivery methods

{type="medium" sorted="desc"}
Redemption URL
: Keep the email address and mobile number empty if you want to deliver the gift card to the recipient yourself. You
will receive a redemption URL in the response that you can provide to the
recipient.

Sent directly
: Provide an email address and or mobile number if you want to leave delivery of the gift card to us. We will
automatically send the gift card to the recipient details you provide.

## Request

```http
POST %url%gift-cards
```

> Make sure to provide the value in the smallest unit of the currency. For example, 1000 for £10.00.
>
{style="note"}

### Example request payload - Recipient choice

You define the available brands and the currency of the gift card by creating a template inside your account.

```json
{
  "type": "recipient_choice",
  "value": 1000,
  "template_id": "9af0e1ce-c130-4aac-83dc-4144d2b1591b",
  "recipient_email": "user@example.com",
  "recipient_mobile_number": "+440000000000",
  "idempotency_key": "unique_key_1"
}
```

> Exclude the `recipient_email` and `recipient_mobile_number` if you want to deliver the gift card to the recipient
> yourself.

> The value of the gift card needs to be supported by the template you are using. You can see the available
> denominations on the template object. [Read more](Template-object.md#allowed_denominations)
>
{style="warning"}

### Example request payload - Direct

You need to provide the ID of the brand you want to create this gift card for as well as a currency.

```json
{
  "type": "direct",
  "value": 1000,
  "recipient_email": "user@example.com",
  "recipient_mobile_number": "+440000000000",
  "idempotency_key": "unique_key_1",
  "brand_id": "9af0e1ce-c130-4aac-83dc-4144d2b1591b",
  "currency": "GBP"
}
```

> Exclude the `recipient_email` and `recipient_mobile_number` if you want to deliver the gift card to the recipient
> yourself.

> The value of the gift card needs to be supported by the brand you are using. You can see the available
> denominations on the brand object. [Read more](Brand-object.md#allowed_denominations)
>
{style="warning"}

## Response

> The `redemption_url` is the URL you can use to direct the user to redeem the gift card.
> The attributes in this object are the same provided in all giftcard responses.
>

<include from="Gift-card-object.md" element-id="gift-card-object"></include>
