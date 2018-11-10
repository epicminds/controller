# controller

The controller keeps things in order.

## REST API

### List Routes

POST /v1/list-routes
```javascript
{
  "variables": {
    "filter": {
      "type": "{name|region|sponsor|theme|location}",
      "text": ""
    },
    "first": 100,
    "after": ""
  }
}
```

200
```javascript
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
  "route": {
    "id": "a36f3ccc-307a-4147-b4b4-d5ecd884dd72",
    "icon": "data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZG",
    "name": "Lorem Ipsum",
    "description": "Excepteur sint occaecat cupidatat non proident",
    "points": [{
      "order": 0,
      "name": "Sed ut perspiciatis",
      "position": {
        "latitude": "54.597285",
        "longitude": "-5.9375"
      }
    },
    {
      "order": 1,
      "name": "Sed ut perspiciatis",
      "position": {
        "latitude": "54.597285",
        "longitude": "-5.9375"
      }
    }]
  }
}
```
