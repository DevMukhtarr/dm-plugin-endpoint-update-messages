# Update Messages
## Authentication:
This api is basically used to get updated messages.
## API methods:
- GET

## End Points:
base url : https://dm.zuri.chat/docs/v1
### /updatemessage
- **Endpoint**: updatemessage/{id}
- **Method**: GET
- **Description**: Used to get an updated message immediately when called, A **message id** is the only required parameter to do this.

#### how to get updated messages
- use the endpoint **https://dm.zuri.chat/api/v1/updatemessage/{id}.**
- use a valid message id in the endpoint.
- you should get the message which is attached to the id.

##### Example: 

```
 https://dm.zuri.chat/api/v1/updatemessage/6141c56d9fd1f4f655d444fe
```
<hr />

##### response:

```json
code:200
 	
Response body
Download
{
  "_id": "6141c56d9fd1f4f655d444fe",
  "created_at": "2021-09-15T10:03:44.912000Z",
  "media": [],
  "message": "testing endpoints",
  "pinned": false,
  "read": false,
  "room_id": "613b2db387708d9551acee3b",
  "saved_by": [
    "string"
  ],
  "sender_id": "lkdl049052098509292",
  "threads": [
    {
      "created_at": "2021-09-15T10:03:44.912000Z",
      "media": [],
      "message": "does it work",
      "message_id": "613f55f96173056af01b4a7b",
      "sender_id": "lkdl049052098509292"
    }
  ]
}
```
<hr />

``` sh
Code: 500
 Description: Error: Internal Server Error
{
  "status": 400,
  "message": "Undocumented"
}
```
<hr />