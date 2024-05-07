# iframe-sample
This repo demonstrates how to add [Hopara](https://hopara.io) visualizations to your project. It's based on the
 [**Hopara Iframe**](https://www.npmjs.com/package/@hopara/iframe) module.

## Running the application

1- Clone the project and install the node dependencies.

```shell
$ npm install
```

2- Configure the environment with the clientId and clientSecret provided by the [Hopara](https://hopara.io) support team.

```javascript
const clientId = "your-hopara-client-id"
const clientSecret = "your-hopara-client-secret"
```
> :warning: In a production environment the access token request should take place on the back-end. This shared secret gives full control over your account.

3- Now you're ready to start the application:

```shell
$ npm start
```

## @hopara/iframe module
You can further customize the integration by changing the [@hopara/iframe](https://www.npmjs.com/package/@hopara/iframe) component props.

```javascript
document.addEventListener('DOMContentLoaded', function () {
  const hopara = Hopara.init({
    accessToken: 'your-access-token',
    visualization: 'sample',
    targetElementId: 'hopara-app-container-id'
  })
})
```

Additional information on this component is available at [@hopara/iframe](https://www.npmjs.com/package/@hopara/iframe).


