# Quick Photo Album
A front-end-only approach to creating quick photo albums, powered by Cloudinary for image management, organisation, manipulation, optimisation and delivery.


1) The page initially loads a placeholder tags and content
2) Querystring parameter for 'album' drives the page logic
3) A /list API request is made to Cloudinary based on the 'album' value
4) JSON response is returned, and parsed to manipulate the DOM accordingly, including image requests
5) Images are subsequently requested from Cloudinary


** Notes **
1) Cloudinary provides generous free accounts which could be sufficient to power many projects, but if your storage, bandwidth or transforms exceed the available free credits, there are likely to be costs in utilising the service further 
2) /list API is NOT enabled by default on Cloudinary accounts