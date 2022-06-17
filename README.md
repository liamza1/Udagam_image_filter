# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

THe Image fitler section works on taking a public image adding a filter to it and then returnng the new filtered image

## Tasks
  Two filter end points have been created to filter the image submitted relying on JIMP processing 
  /FilterImage which adds a Greyscale filter to the image.
  /Invertedimage which inverts the image colours.

## Postman collection (image filter requests)

  the postman Collection is divided in four sections, one for each endpoint in each enviroment with the {HOST} and {EBHOST} Values set accordingly.
  each cotainers the base testing for:
  1. a public access image :status(200)
  2. a non public image :status(500)
  3. no image url :status(400)
  4. no authentication :status(401)

### Setup Node Environment

You'll need to create a new node server. Open a new terminal within the project directory and run:

1. Initialize a new project: `npm i`
2. run the development server with `npm run dev`

### Elastic BeanStalk EndPoint

Deployment Image found in Deployment ScreenShots folder


## Stand Out (Optional)

### Authentication

Prevent requests without valid authentication headers.
Bearer token Imcluded in Postman collection under Variable {{Token}}


