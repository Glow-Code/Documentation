# Get gift card

Get a gift card by its ID.

## Endpoint

```http
POST %url%gift-cards/{id}
```

## Response

> This endpoint will return a single [gift card object](Gift-card-object.md).
>
> If the gift card does not exist, the API will return a `404 Not Found` error.
