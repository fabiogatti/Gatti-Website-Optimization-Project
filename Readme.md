## New Website Performance Optimization portfolio project

Name: Fabio Alessandro Gatti
Email: lucario94@hotmail.com

Documentation for the changes made on the final project

1. For the index.html file here's what i did:
	-Minify html, css and js
	-Compress images
	-Inline css and set js file to async
	-Use cache.apcache file to load to cache all files for index.html and subsquent pages
	-Use the .htaccess file to make use of the deflate tool to compress them when sent

	The initial score that pagespeed gave for the index.html file was 72/100 (mobile) and 75/100 (desktop).
	The final score that pagespeed gave for the index.html file was 94/100 (mobile) and 96/100 (desktop).

	Note: I could've set the following code on the .htaccess file, but i didn't know how to fix an error with the fonts located on the inlined css in the index.html file
		<FilesMatch "\.(css|jpg|jpeg|png|js)$">
			ExpiresActive on
    		Header set Cache-Control "max-age=604800, public"
		</FilesMatch>
	This way i would've had a 100/100 score on pagespeed website, but only 73/100 for user experience because of the fonts error.

2. For the pizza exercise (main.js) here's what i did:
	-Modify 'changePizzaSizes' function so it doesn't take so much to resize the pizzas (Description: line 451;Old code commented: line 456; New code: 463)
	-Modify 'updatePositions' function so it doesn't take so much to move the background pizzas (Description: line 513;Old code commented: line 521; New code: 528)

Note: I used wamp to set the localhost, and then i executed the server with the ngrok file.

Thanks for taking the time to read and evaluate my project.