# quickalbum

A simple front-end-only approach to create quick photo albums leveraging Cloudinary for image management, organisation, manipulation, optimisation and delivery

The page initially loads placeholder markup, everything after that is added to the page using javascript.

Querystring are passed in to drive the 'cloud', 'album' and language preferences for the Quick Album (the querystring is parsed by javascript)

Javascript is used to request 2 JSON files from Cloudinary - these leverage the cloud and album from the querystring.
1) is of the form of a /list/<tag> request and returns details of assets matching the specified tag, which drives the contents of the album
2) is a seperate <tag>-album-details.json file seperately uploaded to contain the title and descriptive text for the album

Based on the JSON responses from these two requests we use vanilla javascript to update the DOM, creating the semantic markup for title, introduction, and a series of images. The asset metadata can be used to manage the Alt tags for each image, and rhe language preference is used to determine which language variant of the metadata to map to.

Image elements follow responsive images approaches for making the media loading more optimal

ToDo - add a js gallery feature for image zoom

** note ** Cloudinary provides generous free accounts which could be sufficient to power many projects, but if your storage, bandwidth or transforms exceed the available free credits, there are likely to be costs in utilising the service further 
