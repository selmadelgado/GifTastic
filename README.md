# GifTastic
A dynamic webpage that calls the GIPHY API and uses JavaScript and jQuery to change the HTML of the site.

Live Project:
https://selmadelgado.github.io/GifTastic/

Summary:
The webpage  automatically loads five pre-made buttons featuring my favorite Pixar Characters. When a button is clicked, 10 of the most relevant gifs populate below.   The gifs can start and stop animating by simply clicking on them.

If your favorite Pixar character is not displayed, you can make your own button with your own favorite character.

Technical Details:
The Giftastic app was created using a combination of HTML, CSS, JavaScript, jQuery and Ajax. 

     It uses jQuery event handlers to detect when a user clicks a button and extract the name of the cartoon show attached to it. 

     The program then encodes the cartoon show title and a ratings limit (I set this to "PG" to only receive family-friendly content) in an Ajax request to the GIPHY API. Upon receiving this request, the GIPHY API sends back a JSON object with data for ten GIFs that meet the query's parameters. 

     The program then extracts the ratings and still-image URLs for each GIF and uses jQuery to display the images and associated ratings to the user. Within each HTML image tag created by jQuery, the program encodes URLs for the animated and still versions of the GIF as well as the image's current state ("still" or "animated"). 

     Additionally, the program attaches a jQuery click handler that switches the image's state and updates the src attribute with either the still or animated URL. This gives users the ability to toggle between the two versions of each GIF by clicking on it.