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
7) Additionally a light box also enables images to be seen bigger, including fullscreen, and also a slideshow
8) Alt text can also be managed via asset contextual metadata
9) Also including multi-lingual alt-tags


[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https%3A%2F%2Fgithub.com%2Fbseymour%2Fquickphotoalbum) <a href="https://app.netlify.com/start/deploy?repository=https://github.com/bseymour/quickphotoalbum">
    <img src="https://www.netlify.com/img/deploy/button.svg" title="Deploy to Netlify">
  </a>


++++++++++++++++++++++++++++  
To use with your own account, make 1 change :
live.html 
62: const cloud_name = 'quickalbum'; 
^^ Change this to your Cloudinary cloudname ^^
and ensure you have list API enabled  
++++++++++++++++++++++++++++  


** Notes **
1) Cloudinary provides generous free accounts which could be sufficient to power many projects, but if your storage, bandwidth or transforms exceed the available free credits, there are likely to be costs in utilising the service further 
2) /list API is NOT enabled by default on Cloudinary accounts


Javascript lightbox gallery from:
https://sachinchoolur.github.io/lightgallery.js/
// for commercial usage, please see their license details

Some demo example media via:
https://unsplash.com/
