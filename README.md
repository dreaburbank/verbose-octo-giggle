# verbose-octo-giggle
Squarespace CSS code that I use all the time, not much of a coder so I'm contributing what I do know!

I always tell myself I won't put any custom CSS on the Squarespace sites I'm coding. But then I always do. 

### Some tips
— To identify the code block in Squarespace download the Google Chrome extension [Block ID](https://chrome.google.com/webstore/detail/squarespace-collectionblo/bggpdfnccodbnmcndckmeehdjkjojkde/related?hl=en-US)  
— You have to upgrade the membership one tier to use custom code  
— To edit this you have to go to Design > Custom CSS > 


### Putting borders around images
So cray cray this isn't just built in yet.

section[data-section-id="606d1447c1b66454c1baa821"] .content-wrapper {. 
  content: '';  
    border-top: 3px solid #708238;  
    border-right: 3px solid #708238;  
    border-left: 3px solid #708238;  
    border-bottom: 3px solid #708238;     
    padding: 8vw !important;  
}  

### The TikTok icon
This only works to replace one icon image, I always pick the TikTok one because that's what I use. 
First you have to upload a new image for the TikTok icon where it says "Manage custom files" 

.sqs-svg-icon--wrapper.url div {
    visibility: hidden;
}
.sqs-svg-icon--wrapper.url {
    background-image: url(//your_tiktok_url_from_custom_files.png);
    background-size: cover;
    background-repeat: no-repeat;
}

.icon[aria-label="URL"] svg {
  visibility:hidden;
}
.icon[aria-label="URL"] {
background-image: url(//your_tiktok_url_from_custom_files.png);
    background-size: cover;
    background-repeat: no-repeat;
    transform:scale(1);
}
