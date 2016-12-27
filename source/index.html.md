---
title: Amplo API Reference

language_tabs:
  - shell
  - ruby

toc_footers:
  - Contact Amplo for a Developer Key
  - <a href='https://amploadvance.com'>Company site</a>

includes:
  - users
  - user_addresses
  - user_emails
  - user_phones
  - reports
  - errors

search: true
---

# Introduction

Welcome to the Amplo API! You can access Amplo endpoints which will allow you to create records in Amplo system.  

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

# Authentication

> Use token like this: 2d931510-d99f-494a-8c67-87feb05e1594

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: Token token='2d931510-d99f-494a-8c67-87feb05e1594'"
```

```ruby
require 'rest-client'

RestClient.get('api_endpoint_here',
  {Authorization: "Token token='2d931510-d99f-494a-8c67-87feb05e1594'" } )
```

> Make sure to replace `2d931510-d99f-494a-8c67-87feb05e1594` with your specific API key.

Amplo uses API keys to allow access to the API. You can register for a new API key at our [developer portal](http://api.amploadvance.com).

Amplo expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: 2d931510-d99f-494a-8c67-87feb05e1594`

<aside class="notice">
You must replace <code>2d931510-d99f-494a-8c67-87feb05e1594</code> with your personal API key.
</aside>
