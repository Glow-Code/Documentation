# Sandbox

To help you test your integration with the glow API, we provide a sandbox environment. This environment is a replica of our live environment, but it allows you to test your integration without
affecting your live account or occurring any costs.

To make use of the sandbox environment, you need to use the following URL:

```http
https://sandbox.glow.net/api/v1/
```

You will need to create a token for the sandbox environment. You can do this by visiting the developer section of your account and creating a new token. Once you have a token, you can use it to access
the sandbox environment.

```Authorization: Bearer <token>```

Once you are ready to go live, you can switch to the live environment by using the following URL:

```http
https://api.glow.net/api/v1/
```

You will need to create a new token for the live environment. You can do this by visiting the developer section of your account and creating a new token.
You need to check the box to indicate that you want to create a production token.

> Only your account owner can create a production token.
>
{style="warning"}
