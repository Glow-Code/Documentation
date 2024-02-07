# Template object

The template object is the same format when returned from any endpoint that returns a template. The template object
has the following structure:

<snippet id="template-object">

```json
{
  "id": "9b45b8d6-3c33-43cd-bac5-a635ce1a81df",
  "title": "You have a new reward",
  "message": "Enter a message for the Gift Card recipient to make it more personal!",
  "name": "You have a new reward",
  "currency": "GBP",
  "brands": [
    {
      "id": "9aed3937-9dad-43b8-b93d-7a07c646185c",
      "name": "Wallmart",
      "slug": "wallmart",
      "display_name": "Wallmart",
      "description": null,
      "created_at": "2023-12-24T16:49:38.000000Z",
      "updated_at": "2024-02-06T16:22:41.000000Z"
    },
    {
      "id": "9aed3937-9b59-4c43-9980-129186ae13e9",
      "name": "Xbox",
      "slug": "xbox",
      "display_name": "Xbox",
      "description": null,
      "created_at": "2023-12-24T16:49:38.000000Z",
      "updated_at": "2024-02-06T16:22:41.000000Z"
    }
  ],
  "allowed_denominations": [
    {
      "amount": "1000",
      "currency": "GBP",
      "formatted": "£10.00"
    },
    {
      "amount": "2000",
      "currency": "GBP",
      "formatted": "£20.00"
    }
  ],
  "created_at": "2024-02-06T16:39:20.000000Z",
  "updated_at": "2024-02-06T16:39:20.000000Z"
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
        <td>id</td>
        <td>string</td>
        <td>The id of the template</td>
</tr>
    <tr>
        <td>title</td>
        <td>string</td>
        <td>The title of the template</td>
</tr>
    <tr>
        <td>message</td>
        <td>string</td>
        <td>The message of the template</td>
</tr>
    <tr>
        <td>name</td>
        <td>string</td>
        <td>The name of the template</td>
</tr>
    <tr>
        <td>currency</td>
        <td>string</td>
        <td>The currency of the template</td>
</tr>
    <tr>
        <td>brands</td>
        <td>array</td>
        <td>The brands available for the template</td>
</tr>
    <tr id="allowed_denominations">
        <td>allowed_denominations</td>
        <td>array</td>
        <td>The gift card values that are available when purchasing a gift card.

```json
{
  "amount": "1000",
  "currency": "GBP",
  "formatted": "£10.00"
}
```

</td>
</tr>
    <tr>
        <td>created_at</td>
        <td>string</td>
        <td>The date the template was created</td>
</tr>
    <tr>
        <td>updated_at</td>
        <td>string</td>
        <td>The date the template was updated</td>
</tr>
</table>


</snippet>