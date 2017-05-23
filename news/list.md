# NEWS LIST
-----------

## Request

    GET /api/v1/news?linked=users


## Response

```javascript

    {
        "status": 1,
        "data": [
            {
                "id"          : "accd97828b241d12d121c1"
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
            },
            {
                "id"          : "accd97828b241d12d121c1"
                "title"       : "Title2",
                "subtitle"    : "Subtitle2",
                "text"        : "Text2",
                "image"       : "url/to/img2",
                "isPublished" : "true",
                "createdAt"   : "2016-02-23T13:41:54.457Z",

                "links": {
                    "authors": [
                        {"type": "users", "id": "accd97828b241d12d121c143999"},
                    ]
                }
            }
        ],

        "linked": {
            users: [{
                "id"          : "accd97828b241d12d121c143211",
                "email"       : "john@mail.com",
                "firstName"   : "john",
                "secondName"  : "smith"
            },{
                "id"          : "accd97828b241d12d121c143244",
                "email"       : "alise@mail.com",
                "firstName"   : "alise",
                "secondName"  : "smith"
            },{
                "id"          : "accd97828b241d12d121c143999",
                "email"       : "bob@mail.com",
                "firstName"   : "bob",
                "secondName"  : "smith"
            }]
        },

        "meta": {
            "totalCount": 2,
            "filteredCount": 2,
            "limit": 20,
            "offset": 0
        }
    }

```