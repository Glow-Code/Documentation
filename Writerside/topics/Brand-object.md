# Brand object

The brand object is the same format when returned from any endpoint that returns a brand. The brand object
has the following structure:

<snippet id="brand-object">

```json
{
  "id": "9aed3938-59b9-4508-95c6-982a9baa7dcf",
  "name": "Example brand",
  "slug": "example-brand",
  "display_name": "Example Brand",
  "currency": "GBP",
  "description": null,
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
  "created_at": "2023-12-24T16:49:39.000000Z",
  "updated_at": "2024-02-06T16:22:41.000000Z"
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
        <td>The id of the brand</td>
    </tr>
    <tr>
        <td>name</td>
        <td>string</td>
        <td>The name of the brand</td>
    </tr>
    <tr>
        <td>slug</td>
        <td>string</td>
        <td>The slug of the brand</td>
    </tr>
    <tr>
        <td>display_name</td>
        <td>string</td>
        <td>The display name of the brand</td>
    </tr>
    <tr>
        <td>currency</td>
        <td>string</td>
        <td>The currency of the brand</td>
    </tr>
    <tr>
        <td>description</td>
        <td>string</td>
        <td>The description of the brand</td>
    </tr>
    <tr id="allowed_denominations">
        <td>allowed_denominations</td>
        <td>array</td>
        <td>The allowed denominations for the brand.

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
        <td>The date and time the brand was created.</td>
    </tr>
    <tr>
        <td>updated_at</td>
        <td>string</td>
        <td>The date and time the brand was last updated.</td>
    </tr>

</table>


</snippet>