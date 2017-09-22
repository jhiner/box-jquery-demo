# Auth0 Box API - jQuery Demo

This demo shows how users can authenticate with Auth0 and request an `access_token` for Box. This access token in turn allows you to interact with the [Box Platform API](https://developer.box.com/reference#api-docs-directory).

## Configuration

 1. [Create a new "Single Page Web Application"](https://manage.auth0.com/#/clients)
 2. Configure `http://localhost:7001` as the Allowed Callback URL for this application
 3. Go to the [Box Developer Console](https://app.box.com/developers/console) and enable CORS for `http://localhost:7001`
 4. Setup a new API in Auth0 for Box. You can use the configuration information you downloaded in the JSON file from the [Box Developer Console](https://app.box.com/developers/console). Note the identifier for the config file.
 4. Copy config-sample.json as config.json, and update this file with the information of your Auth0 Client:

```
{
  "AUTH0_DOMAIN": "you.auth0.com",
  "AUTH0_CLIENT_ID": "gKYI3eXfKZ.........",
  "CALLBACK_URL": "http://demo.com:7001/",
  "BOX_API_IDENTIFIER": "my-box-api"
}
```

## Running the demo

```
npm install
node server
```

Then simply navigate to [http://localhost:7001/](http://localhost:7001/``)
