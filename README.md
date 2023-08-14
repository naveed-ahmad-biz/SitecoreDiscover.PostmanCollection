# SitecoreDiscover.PostmanCollection
A Postman API client collection for API calls related to Sitecore Discover. For more information, read the <a href="https://naveed-ahmad.com/2023/08/14/introducing-postman-collection-for-sitecore-discovers-rest-api/"  target="_blank">blog</a> 

## How to use this postman collection
- Import the two scripts into Postman API client.
- Copy customer key and API keys from Sitecore Discover's CEC portal.
- Generate token using one of the authentication API POST request.
  - Copy the access_token generated in the previous call in the corresponding variable of the envrionment file.
- Make subsequent requests from collection.

## Environment File
The following are the variables in the environment file:

| Variable Name		| Type	| Comments	| Example
| :------------- 	| :----- | :------------- | :-------
|customer_key		|string	|The customer key is as per the CEC portal. Copy the value from the CEC portal.	|11111-222333444
|search_api_key		|string	|Search API Key. You may have one key for all or a separate key for each API end point. Copy the value from the CEC portal.	|01-9c61b…09bc
|event_api_key		|string	|Event API Key. You may have one key for all or a separate key for each API end point. Copy the value from the CEC portal.	|01-9c61b…09bc
|feed_api_key		|string	|Feed API Key. You may have one key for all or a separate key for each API end point. Copy the value from the CEC portal.	|01-9c61b…09bc
|services_api_key	|string	|Services API Key. You may have one key for all or a separate key for each API end point. Copy the value from the CEC portal.	|01-9c61b…09bc
|server_api_host	|string	|Server API host, as mentioned in your CEC portal. Copy the value from the CEC portal.	|https://api.rfksrv.com
|scope_search		|string	|Pre-defined value for scope, do not change this value.	|search-rec
|scope_event		|string	|Pre-defined value for scope, do not change this value.	|event
|scope_feed		|string	|Pre-defined value for scope, do not change this value.	|feed
|scope_services		|string	|Pre-defined value for scope, do not change this value.	|services
|access_token_search_rec|string	|The user-generated access token value for Search API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|access_token_feed	|string	|The user-generated access token value for Feed API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|access_token_events	|string	|The user-generated access token value for Event API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|access_token_services	|string	|The user-generated access token value for Services API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|refresh_token_search_rec|string|The user-generated refresh token value for Search API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|refresh_token_feed	|string	|The user-generated refresh token value for Feed API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|refresh_token_events	|string	|The user-generated refresh token value for Events API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|refresh_token_services	|string	|The user-generated refresh token value for Services API. Copy the value after generating the token via Postman.	|eyJ0e…gqag
|access_token_expiry	|string	|Length of token expiry in milliseconds. Default to 86400000 (a day).	|86400000
|refresh_token_expiry	|string	|Lenght of refresh token in milliseconds. Default to 604800000 (a week)	|604800000

## Collection File
The postman collection file is divided into four top level sections:

- Authentication
- Search & Recommendations
- Events
- Incremental Feed


