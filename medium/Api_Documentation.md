## API for Blog Testing App
---

The file consist of how to use API to perform CRUD Operations on the blog app.

``
https://dashingtoothpaste.backendless.app/api/data/Blog_Data``

#### Create Operation (Post) - 
- Hit the given API URL with POST method
- Sample Request Body 
```json 
{
    "author": "xyz",
    "title": "Post from api",
    "content": "A test to post data from api"
}
```

#### Read Operation (Get) - 
- Hit the given URL API with GET method
- Sample Response Body
```json
{
	"blog_id": 10,
	"author": "xyz",
	"created": 1634290414000,
	"___class": "Blog_Data",
	"ownerId": null,
	"title": "Post from api",
	"updated": null,
	"objectId": "55F1A506-59D8-4BA0-B635-8B6406A2B201",
	"content": "A test to post data from api"
}
```
#### Update Operation(Update) - 

- Hit the given API URL with UPDATE method.
- Sample Request Body
```json
{
    "objectId": "1D4C8B70-C073-41D8-84EE-A4D16FC06F55",
    "author" : "ABC"
}
```
- Get the post objectId that needs to be updated.
- Mention the data need to update along with objectId.

#### Delete Operation(Delete) - 
- Hit the given API URL with DELETE method
- Sample Request Body
```json 
{
  "objectId": "55F1A506-59D8-4BA0-B635-8B6406A2B201"
}
```
- The particular post with given objectId would be deleted if exist.


## Later Updates:-

1. How to fetch a single post.
2. Search/Filter post on URL params.
3. Get the sorted data from backend.
