![Fitness](https://www.gstatic.com/images/branding/product/1x/googleg_32dp.png)

# UnOfficial Fitness v1 Samples for PHP

## API Description

Stores and accesses user data in the fitness store from apps on any platform.

[Official Documentation](https://developers.google.com/fit/rest/)

## Sample Description

These samples show how to access the [Fitness v1](https://developers.google.com/fit/rest/) with the Official [Google PHP client library](https://github.com/google/google-api-php-client)

Tutorials to go along with some of these samples can be found on [www.daimto.com](http://www.daimto.com/)

## Developer Documentation

* [Google API client Library for .NET - Get Started](https://developers.google.com/api-client-library/dotnet/get_started)

* [Supported APIs](https://developers.google.com/api-client-library/dotnet/apis/)

### Credentials 

#### Oauth2

Create credentials

Open the Credentials page.

* Click [Create credentials](https://console.developers.google.com/apis/credentials) and select OAuth client ID
* For the Application type select Web application.
* Name the client ID PHPSample and click Create.
* Leave the Authorized JavaScript origins blank, it is not needed for this tutorial.
* Set the Authorized redirect URIs to http://localhost:8080/oauth2callback.php
* Click Create.
From the [Credentials](https://console.developers.google.com/apis/credentials) page click into the newly created client ID, and click Download JSON and save it as client_secrets.json; you will need it later.

#### Service account

Note: not all APIs support service accounts.

* Open the [Service accounts](https://console.developers.google.com/permissions/serviceaccounts) page. If prompted, select a project.
* Click Create service account.
* Download the json file name it service-account.json; you will need it later
* In the Create service account window, type a name for the service account, and select Furnish a new private key. If you want to [grant G Suite domain-wide authority](https://developers.google.com/identity/protocols/OAuth2ServiceAccount#delegatingauthority) to the service account, also select Enable G Suite Domain-wide Delegation. Then click Create.
* place service-account.json in the directory along with your code.

Include the following line in your script to include service account authencation code.

require_once __DIR__ . '/ServiceAccount.php';





#### Public API Key

Note: Public API keys can only be used to access public data.

### Installing Composer

The preferred method is via https://getcomposer.org. Follow the installation instructions https://getcomposer.org/doc/00-intro.md 
if you do not already have composer installed.

Once composer is installed, execute the following command in your project root to install this library:

```
composer require google/apiclient:^2.0
```

### Usage


