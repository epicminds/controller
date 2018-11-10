# controller

The controller keeps things in order.

## REST API

### List Routes

Request
```javascript
POST /v1/list-routes
{
  "filterType": "{name|region|sponsor|theme|location|type}",
  "filterText": "",
  "first": 100,
  "after": "" # cursor value
}
```

Reponse
```
200
{ 
  "pageInfo": {
    "startCursor": "",
    "endCursor": "",
    "hasNextPage": true
  },
  "routes": [{
    "id": "a36f3ccc-307a-4147-b4b4-d5ecd884dd72",
    "icon": "data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZG",
    "name: "Lorem Ipsum",
    "description": "Excepteur sint occaecat cupidatat non proident"
  },
  {
  "id": "a36f3ccc-307a-4147-b4b4-d5ecd884dd72",
    "icon": "data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZG",
    "name: "Lorem Ipsum",
    "description": "Excepteur sint occaecat cupidatat non proident"
  }]
}
```

### Get Route

Request
```
GET /v1/route/{id}
```

Response
```
{

}
```
