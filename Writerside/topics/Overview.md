# Authentication

To securely access Glow's APIs, we use a method called Bearer Token Authentication. You can obtain a Bearer token from the developer section of your account. Once you have a token, you can use it to
access our APIs:

```Authorization: Bearer <token>```

Our server will validate the Bearer token and, if it is valid, will process the request. If the token is missing, invalid or expired, an error message will be returned.

This method ensures secure communication and prevents unauthorized access to the resources of your account.

> Remember: Protect your Bearer tokens to ensure the security of your application. Tokens are sensitive data and should never be stored in publicly accessible areas.
>
{style="warning"}

### Example Request

```cURL
curl --request GET \
  --url %url% \
  --header 'Accept: application/json' \
  --header 'Authorization: Bearer 2|UICo3K96IGIwUsgds8qoKFOW1IEnSSMS7pgNAeTBc94b54ca'
```
