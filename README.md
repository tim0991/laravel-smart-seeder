```json
{
    "_mapping": {
        "users": "\\App\\Models\\Users",
        "profile": "\\App\\Models\\UserProfile",
        "attributes": "\\App\\Models\\Attributes"
    },
    "users": [
        {
            "username": "xxx",
            "password": "xxx",
            "!profile": {
                "relation": "hasone"
            },
            "!attributes": {
                "relation": "belongsToMany",
                "table": "user_attrs",
                "random": 1,
                "limit": [1, 2],
                "fields": {
                    "vid": {
                        "relation": "hasMany",
                        "random": "5"
                    }
                }
            }
        }
    ],
    "profile": {
        "name": "xiaoming",
        "age": "12",
        "sex": "1"
    },
    "attributes": [
        {
            "name": "a1",
            "values": [
                {
                    "name": "v1",
                    "value": "v1"
                },
                {
                    "name": "v2",
                    "value": "v2"
                },
                {
                    "name": "v3",
                    "value": "v3"
                }
            ]
        },
        {
            "name": "a2",
            "values": [
                {
                    "name": "v1",
                    "value": "v1"
                },
                {
                    "name": "v2",
                    "value": "v2"
                },
                {
                    "name": "v3",
                    "value": "v3"
                }
            ]
        }
    ]
}
```
