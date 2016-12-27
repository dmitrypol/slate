# Users

## Get All Users

```shell
curl "http://api.amploadvance.com/v2/users"
  -H "Authorization: Token token='2d931510-d99f-494a-8c67-87feb05e1594'"
```

```ruby
require 'rest-client'

RestClient.get('http://api.amploadvance.com/v2/users',
  {Authorization: "Token token='2d931510-d99f-494a-8c67-87feb05e1594'" } )

```

> The above command returns JSON structured like this:

```json
[
  {
    "id": "564a958769702d34930007a4",
    "first-name": "Jane",
    "last-name": "Doe",
    "email": "jane.doe@email.com"
  },
  {
    "id": "564a958769702d34930007a2",
    "first-name": "John",
    "last-name": "Smith",
    "email": "john.smith@email.com"
  }
]
```

This endpoint retrieves all users.

### HTTP Request

`GET http://api.amploadvance.com/v2/users`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
limit | 20 | Maximum is 50
offset | 0 |

<aside class="success">
Remember — you must authenticate to access the API.
</aside>

## Get a Specific User

```shell
curl "http://api.amploadvance.com/v2/users/ID"
  -H "Authorization: Token token='2d931510-d99f-494a-8c67-87feb05e1594'"  
```

```ruby
require 'rest-client'

RestClient.get('http://api.amploadvance.com/v2/users/ID',
  {Authorization: "Token token='2d931510-d99f-494a-8c67-87feb05e1594'" } )
```

> The above command returns JSON structured like this:

```json
{
  "id": "564a958769702d34930007a4",
  "first-name": "Jane",
  "last-name": "Doe",
  "email": "jane.doe@email.com"
}
```

This endpoint retrieves info a specific user

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://api.amploadvance.com/v2/users/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the user to retrieve
