# ![LOGO](logo.png) Taxrates.io **flow**ground Connector

## Description

A generated **flow**ground connector for the Taxrates.io API (version 3.0).

Generated from: https://api.apis.guru/v2/specs/taxrates.io/3.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:21+03:00

## API Description

Taxrates.io API - the successfully streamlined tax rates monitoring process. Use 'Expand operation' link on the right to see details. Start with authentication: get your token and generate authorization string. We recommend using <a href='https://www.getpostman.com/' target=_new>Postman</a> when discovering our API. Happy using!

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Authorization endpoint

> This is the second endpoint you have to hit. When you got your token here you can generate your Bearer authorization header. The header will be used to authorize every API call.

*Tags:* `Authentication`

#### Input Parameters
* `domain` - _required_ - Domain name: api.taxrates.io
* `token` - _required_ - The token you got from <<token>> endpoint
* `clientscope` - _required_ - You have to use api_member as a scope.

### Token generating URL

> This the very first URL you must hit when you want to use taxrates.io API. When you got your Client ID key and Client Secret key you are able to use our API resources.

*Tags:* `Authentication`

#### Input Parameters
* `domain` - _required_ - Domain name: api.taxrates.io
* `clientid` - _required_ - Your Client ID goes here. Check the dashboard if you do not know your Client ID.
* `clientsecret` - _required_ - Your Client Secret key goes here. Check the dashboard if you do not know your Client Secret key.
* `clientscope` - _required_ - You have to use api_member as a scope.

### Get tax rates by address

> This endpoint returns tax rates for the country based on the address provided

*Tags:* `Tax service`

#### Input Parameters
* `domain` - _required_ - Domain name: api.taxrates.io
* `filter` - _optional_ - You can filter your taxes by one of following types: 'standard', 'reduced', 'second reduced', 'third reduced' and 'super reduced'.

### Returns tax rate for selected country

> This endpoint returns all available tax rates for selected country

*Tags:* `Tax service`

#### Input Parameters
* `domain` - _required_ - Domain name: api.taxrates.io
* `country_code` - _required_ - Country code alpha 2
* `filter` - _optional_ - You can filter your taxes by one of following types: 'standard', 'reduced', 'second reduced', 'third reduced' and 'super reduced'.

### Tax rates by geolocation based on Customer IP address

> This endpoint will return tax rates for country discovered based on Customer's IP address

*Tags:* `Tax service`

#### Input Parameters
* `domain` - _required_ - Domain name: api.taxrates.io
* `ip` - _required_ - Customer's IP address
* `filter` - _optional_ - You can filter your taxes by one of following types: 'standard', 'reduced', 'second reduced', 'third reduced' and 'super reduced'.

### Get all tax rates

> This method returns all tax rates configured on Member's account

*Tags:* `Tax service`

#### Input Parameters
* `domain` - _required_ - Domain name: api.taxrates.io
* `filter` - _optional_ - You can filter your taxes by one of following types: 'standard', 'reduced', 'second reduced', 'third reduced' and 'super reduced'.
* `zip` - _optional_ - You must provide a zip code if one of your selected countries is United States and you've had selected a state on your Taxrates.io member's dashboard.

## License

**flow**ground :- Telekom iPaaS / taxrates-io-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
