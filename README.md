# ImageProcessing

Architecture
![alt tag](http://i.imgur.com/VaSF6gg.jpg?1)


GET /image - Returns a list of all images

GET /image/:id - Returns a image with the given id

POST /image - Save image to CDN or convert to base64 and sev in DB as string

PUT /image/:id / specifyAction - Retrieve image with the passed Id, then checks for its action, i.e. crop/saturate/normalize and then do processing based on the passed Data

Another way is to create separate API for all 3 actions like for crop image
PUT /image/:id / cropImage - Retrieve image with the passed Id, then crop it based on the passed Data

DELETE /image/:id - Deletes a comment with the given id
