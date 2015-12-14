# Share social media buttons
Add social media buttons to share articles in your website. Preview [here](http://mahcode.com/share_article/)

Buttons:

- Facebook
- Twitter
- Google+
- LinkedIn
- Pinterest
- Tumblr

![Buttons](http://mahcode.com/share_article/1.PNG)

##Requirements
-jQuery

##Steps
###Step 1
In order to use these buttons you need to include the OpenGraph Meta Tags in your page, you can find them in the ``index.html`` file.
###Step 2
Replace the content in brackets for each meta tag with the information of your article. For example:
```html
<meta name="description" 				content="The first thing Game Of Thrones released to tease its upcoming sixth season was a poster featuring Jon Snow.">
<meta name="author" 					content="Mahsource">
<meta property="og:locale" 				content="en_EN"/>
<meta property="og:type" 				content="article"/>
<meta property="og:title" 				content="Game of Thrones Season 6: Tease"/>
<meta property="og:description" 		content="The first thing Game Of Thrones released to tease its upcoming sixth season was a poster featuring Jon Snow."/>
<meta property="og:url" 				content="http://mahcode.com/share_article/"/>
<meta property="og:site_name" 			content="mahcode.com"/>
<meta property="article:publisher" 		content="https://www.facebook.com/Mahcode-849841581779986"/>
<meta property="article:published_time" content="2015-12-10T02:05:30Z"/>
<meta property="og:image" 				content="http://mahcode.com/share_article/teaser-jon-snow.jpg"/>
  

<meta name="twitter:title" 				content="Game of Thrones Season 6: Tease"/>
<meta name="twitter:description" 		content="The first thing Game Of Thrones released to tease its upcoming sixth season was a poster featuring Jon Snow."/>
<meta name="twitter:image" 				content="http://mahcode.com/share_article/teaser-jon-snow.jpg"/>
<meta name="twitter:site" 				content="@itsmahcode"/>
<meta name="twitter:creator" 			content="@itsmahcode"/>
<meta name="twitter:via" 				content="itsmahcode"/>
<meta name="twitter:card" 				content="photo"/>
<meta name="twitter:url" 				content="http://mahcode.com/share_article/"/>
```

###Step 3
Include the code from ``functions.js`` and  ``style.css`` into your code files.  If you have a main javascript file in your site, then include the code from ``functions.js``. And do the same with the css file. Just copy the styles from ``style.css`` into your main css file.
Then add the following HTML into your page in order to display the buttons

```HTML
<!-- Buttons, Copy this to your Page Article -->
<div class="share-buttons-row">
	<!--Facebook's Button -->
	<div class="share-fb"></div>
	<!--Twitter's Button -->
	<div class="share-twitter"></div>
	<!--Facebook's Button -->
	<div class="share-google-plus"></div>
	<!--Linkedin's Button -->
	<div class="share-linkedin"></div>
	<!--Pinterest's Button -->
	<div class="share-pinterest"></div>
	<!--Tumblr's Button -->
	<div class="share-tumblr"></div>
</div>
```


###and that's it!

###Notes
- If you are working with PHP or ASP.NET you can replace the content in meta tags automatically by printing your variables in the content.

For example in PHP. You can do something like this:

```php
<meta name="description" 				content="<?php echo $article_info['description']; ?>">
<meta name="twitter:title" 				content="<?php echo $article_info['title']; ?>"/>
...
<meta property="og:image" 				content="<?php echo $article_info['main_image']; ?>"/>
```
- Adding the URL of your main image into the ``<meta property="og:image" 				content=""/>`` is not enough, you have to display the image somewhere in your article, otherwise you won't see the "preview image" when you are sharing the image through facebook.
