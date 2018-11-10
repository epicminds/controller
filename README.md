# controller

The controller keeps things in order.

## REST API

### List Routes

Request
```
GET /v1/list-routes/?filterType={name|region|sponsor|theme|location|type}&filterText={string}
```

Reponse
```
[{
  "id": "a36f3ccc-307a-4147-b4b4-d5ecd884dd72",
  "icon": "data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZG",
  "name: "",
  "description": "",
  "downloaded": true
},
{
"id": "a36f3ccc-307a-4147-b4b4-d5ecd884dd72",
  "icon": "data:image/svg+xml;utf8;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZG",
  "name: "",
  "description": "",
  "downloaded": true
}]
```
### Get Route
GET /v1/route/{id}
