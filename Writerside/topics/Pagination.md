# Pagination

When you make a request to an endpoint that supports pagination, the response will include a subset of the data along with `links` and `meta` objects.

### Example response:

```json
{
    "data": [
        ...
    ],
    "links": {
        "first": "https://endpoint?page=1",
        "last": null,
        "prev": null,
        "next": "https://endpoint?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "path": "https://endpoint",
        "per_page": 10,
        "to": 10
    }
}
```

### Links object

The `links` object contains the following keys:

- `first`: The URL of the first page of results.
- `last`: The URL of the last page of results.
- `prev`: The URL of the previous page of results.
- `next`: The URL of the next page of results.

### Meta object

The `meta` object contains the following keys:

- `current_page`: The current page number.
- `from`: The index of the first item on the current page.
- `path`: The base URL of the endpoint.
- `per_page`: The number of items per page.
- `to`: The index of the last item on the current page.

### Example usage

To retrieve the next page of results, make a request to the `next` URL in the `links` object.

```http
GET https://endpoint?page=2
```

