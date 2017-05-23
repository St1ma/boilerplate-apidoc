# NEWS SHOW
-----------

## Request

    GET /api/v1/news/:id


## Response

```javascript

    {
        "status": 1,
        "data": {
            "id"          : "accd97828b241d12d121c143242"
            "title"       : "Title",
            "subtitle"    : "Subtitle",
            "text"        : "Text",
            "image"       : "url/to/img",
            "isPublished" : "false",
            "createdAt"   : "2016-02-23T13:41:54.457Z",


            "links": {
                "authors": [
                    {"type": "users", "id": "accd97828b241d12d121c143211"},
                    {"type": "users", "id": "accd97828b241d12d121c143244"}
                ]
            }
        }
    }

```