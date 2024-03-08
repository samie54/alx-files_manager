Project: Island Perimeter 
Author: Samuel Atiemo

Project Tasks:

0. Redis utils
mandatory
Inside the folder utils, create a file redis.js that contains the class RedisClient.

1. MongoDB utils
mandatory
Inside the folder utils, create a file db.js that contains the class DBClient.

2. First API
mandatory
Inside server.js, create the Express server:

it should listen on the port set by the environment variable PORT or by default 5000
it should load all routes from the file routes/index.js

3. Create a new user
mandatory
Now that we have a simple API, it’s time to add users to our database.

4. Authenticate a user
mandatory
In the file routes/index.js, add 3 new endpoints:

5. First file
mandatory
In the file routes/index.js, add a new endpoint:

POST /files => FilesController.postUpload

6. Get and list file
mandatory
In the file routes/index.js, add 2 new endpoints:

GET /files/:id => FilesController.getShow
GET /files => FilesController.getIndex

7. File publish/unpublish
mandatory
In the file routes/index.js, add 2 new endpoints:

8. File data
mandatory
In the file routes/index.js, add one new endpoint:

GET /files/:id/data => FilesController.getFile

9. Image Thumbnails
mandatory
Update the endpoint POST /files endpoint to start a background processing for generating thumbnails for a file of type image:

Create a Bull queue fileQueue

10. Tests!
#advanced
Of course, a strong and stable project can not be good without tests.

Create tests for redisClient and dbClient.

11. New user - welcome email
#advanced
Update the endpoint POST /users endpoint to start a background processing for sending a “Welcome email” to the user:


