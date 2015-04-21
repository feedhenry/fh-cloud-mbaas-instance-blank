# FeedHenry Hello World MBaaS Server

This is a blank 'push hello world' FeedHenry MBaaS. Use it as a starting point for building your APIs.
It supports CRUD operations on Categories that are used in the console and the mobile app as publish/subscribe
for the push notifications of interest.

# Group Push Hello World API

# category [/category]

'api' endpoint.

## category [GET]

'Category' endpoint.

+ Request (application/json)

+ Response 200 (application/json)
    + Body
            {
              "status": "ok"
              "data": ["category1", "category2"]
            }

## category [POST]

+ Request (application/json)
    + Body
        {
            "name": "new category name"
        }
        
+ Response 200 (application/json)
    + Body
            {
                "status": "ok"
                "message": <entity>
            }
            
## category/:name [DELETE]

