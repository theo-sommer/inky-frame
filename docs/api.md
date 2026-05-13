# API endpoints provided by the backend:

- **Images**
  - **Get all images:** (GET) /images
  - **Get a random image:** (GET) /images/random
  - **Delete image:** (DELETE) /images/:imageId
  - **Upload image:** (POST) /albums/:albumId/images (the image needs to be in a form with the attribute `enctype="multipart/form-data"` and the input should have the attributes `type="file" name="file"`)
- **Albums**
  - **Get all albums:** (GET) /albums
  - **Get album:** (GET) /albums/:albumId
  - **Get a random image in an albums:** (GET) /albums/:albumId/random
  - **Create album:** (POST) /albums (the name should be in the request.body `{name: "New Album"}`)
  - **Update album by id:** (PUT) /albums/:albumId (the name should be in the request.body `{name: "New Name"}`)
  - **Delete album:** (DELETE) /albums/:albumId
- **Display**
  - **Get current pi temperature:** (GET) /display/pi/temp
  - **Update display:** (POST) /display/image (the image id should be in the request.body `{imageId: 12}`)
  - **Get current image:** (POST) /display/image
  - **Update current album:** (POST) /display/album (the album id should be in the request.body `{albumId: 4}`)
  - **Get current album:** (POST) /display/album
