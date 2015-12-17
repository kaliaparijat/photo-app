# slack
A photo app for slack, written in pure javascript.  

PLEASE NOTE:

* This app uses oAuth authentication from Instagram to run itself, accordingly the app's website and redirect URI 
are: http://localhost/slack

* To run this app locally, please fork this repo inside your favorite web root folder in a folder called 'slack'.
It should be browsable here: http://localhost/slack for the app to work correctly.

* Alternately, feel free to register your own app with Instagram and update the credentials inside main.js

Limitations:

1. User must have an instagram account, with at least a handful of pictures loaded so the app can pull that data in
2. User must authenticate app 


Playing with the app:

1. Click a picture, opens in lightbox, 
2. ESC closes lightbox, arrow keys for slideshow navigation


Design decisions:

The App is broken into two key components: The App in itself and a View object that handles all user operations. 
A utility file is available for

Why no Model? 

I chose not to create a separate model object/class. Primarily because the app only reads data from the server (API) and has no
create, update or delete operations. Given this scope, I do not think a model would apply. It's also designed in such a way 
that if in the future there is a need for operations on the data, I can easily pluck this out and create a new model object
with next to negligible refactor for the current app.

Finally, the HTML and CSS design is minimalistic. I went overtime, spending close to 5 hours on this and wanted to wrap this up since the initial expectation was 3 hours. 

All in all, I had a great experience building this using pure Javascript. Thank you! 


