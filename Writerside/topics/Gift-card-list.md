# Listing gift cards

This endpoint allows you to list all the gift cards that have been bought.

> Some gift cards may have child gift cards associated with them. This is the case when a gift card has been split into
> multiple gift cards.
> You can read more about user choice gift cards in the [Purchase gift card](Gift-card-purchase.md#gift-card-types)
> documentation.

## Endpoint

```http
GET %url%gift-cards
```

## Allowed filters

`?filter[type]=recipient_choice`
: Possible values are `direct` and `recipient_choice`. This filter allows you to filter the gift cards by their type.
: *Read more about the different types of gift cards in the [purchase gift card](Gift-card-purchase.md#gift-card-types)
documentation.*

## Response

> This endpoint will return a list of [gift card objects](Gift-card-object.md).
>
> Make sure to checkout our [pagination](Pagination.md) documentation to see how to paginate the response.

