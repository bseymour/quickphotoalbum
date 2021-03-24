# Quick Photo Album
A front-end-only approach to creating quick photo albums, powered by Cloudinary for image management, organisation, manipulation, optimisation and delivery.

Live example : [https://quickphotoalbum.vercel.app/](https://quickphotoalbum.vercel.app/)  
^^ Try searching for: cars, sunsets or motorbikes

1) The page initially loads a placeholder tags and content
2) Querystring parameter for 'album' drives the page logic
3) A /list API request is made to Cloudinary based on the 'album' value
4) JSON response is returned, and parsed to manipulate the DOM accordingly, including image requests
5) Images are subsequently requested from Cloudinary
6) Album details are managed via a seperate .json file {album}-album-details.json


[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https%3A%2F%2Fgithub.com%2Fbseymour%2Fquickphotoalbum)


** Notes **
1) Cloudinary provides generous free accounts which could be sufficient to power many projects, but if your storage, bandwidth or transforms exceed the available free credits, there are likely to be costs in utilising the service further 
2) /list API is NOT enabled by default on Cloudinary accounts. [Read more about the list API](https://cloudinary.com/documentation/advanced_url_delivery_options#client_side_resources)
3) Deploying to services such as Netlify or Vercel can make hosting this project quick and easy, and while both have generous free tiers, please review the limitations and constraints of using these free tiers, and with increased utilisation, could lead to costs.

Javascript lightbox gallery from:
https://sachinchoolur.github.io/lightgallery.js/
// for commercial usage, please see their license details

Demo example media via:
https://unsplash.com/

