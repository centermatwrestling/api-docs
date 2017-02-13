---
title: API Reference

language_tabs:
  - shell
  - java
  - javascript

toc_footers:
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the Centermat Wrestling API! This api is designed to provide a robust engine for developers/desginers to gain access to statistical data for wrestling at all levels of competition. This is the same api that powers our world class [CMW APP](http://app.centermatwrestling.com)


We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Slate](https://github.com/tripit/slate). Feel free to edit it and use it as a base for your own API's documentation.

# Authentication

# Teams

## Get All Teams

```shell
curl -X GET --header 'Accept: application/json' 'http://api.centermatwrestling.com/api/v1/teams?size=100'
```


> The above command returns JSON structured like this:

```json
{
  "content": [
    {
     "id": "1b4a0de8-3a80-4626-8d83-cec53b2e219c",
     "link": "http://api.centermatwrestling.com/api/v1/teams/1b4a0de8-3a80-4626-8d83-cec53b2e219c",
     "name": "Test Team",
     "logoPath": "http://www.centermatwrestling.com/cdn/images/badge.gif",
     "shortName": "T Team",
     "abbr": "TT",
     "conferenceId": "4629276c-786a-4765-8d07-846861aef3bf",
     "levelOfPlayId": "5f454a63-b96d-4403-b55e-0e10acc49b47"
   }
  ],
  "totalPages": 1,
  "totalElements": 1,
  "last": true,
  "numberOfElements": 1,
  "size": 100,
  "number": 0,
  "first": true
}
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://api.centermatwrestling.com/api/v1/teams`

### Query Parameters


