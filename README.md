This is my first open source framework. It's pretty basic but that's the benefit of it.
The code is a simple breakdown of the parallax effect for anyone who doesn't want the hassle of having to edit a tonne of code. It's as simple as duplicating another item tag in the index.html and duplicating the item selector in the style.css. The cool thing is that the site should scale to fit your browser on any screen size, but if you do run into problems the code is setup for you to make changes at proper breakpoints.

Here's the current link to the example site: http://diymanik.pancakeapps.com/Simplax/index.html

Here's some of the code:

The html tag:

<div class="gallery-item" id="item-1"></div>

Just copy, paste this under the list of tags, change the id item number (#) and the page will expand to fit your image.

The css selector:

#item-1 {

	background-image: url(slideshow/simplax-info-1.png);
	background-repeat: no-repeat;
	background-position: center center;
	background-attachment: fixed;
	
	/** Matches the background size to the browser width **/
	-webkit-background-size: cover;
	-moz-background-size: cover;																			    -o-background-size: cover;																				background-size: cover;
	
	height: 675px;
	}

Just copy and paste this under the list of item selectors, change the item number (#), and change the background-url: to the filename of your image name & location. It's that easy.


Extras:

For the more technically savvy there is the option of adding in tags to allow your webpage visitors to go to a specific point on the page.

Just an anchor tag <a href="">Place the name of your link here<a/> in the <nav> element. Finally change the href="" value to the id of the specific gallery element you would like the page to jump to.

The code should look like this:

<nav class="container">
	<div class="logo"></div>

	<a class="cuban-linx" href=""><h3>Example Link 1</h3></a>
	<a class="cuban-linx" href=""><h3>Example Link 2</h3></a>
	<a class="cuban-linx" href=""><h3>Example Link 3</h3></a>
</nav>


You may also want to change the site title to match the name of your project.
Just change the text between the <title>Simplax.css</title> and <h1>Change the name of your project here</h1>.

Also if you want to change the logo just go to the #logo selector in style.css and change the background-image: url();
As well you should change the width and the height to your preferred pixel size.

The code should look like this:

#logo {
	background-image: url(images/jm-logo-blue-circle.png);
	background-repeat: no-repeat;
	background-position: center center;
	background-attachment: fixed;
	
	/** Matches the background size to the browser width **/
	-webkit-background-size: cover;
	-moz-background-size: cover;
	-o-background-size: cover;
	background-size: cover;

	height: 75px;																					    width: 75px;

}

That's pretty much the basics of what are available to use. The whole point is to be as simple as possible so that Designers can design and drop their images into the code with ease. Any extras like transitions or js are up to the more capable users to add-on. I hope this is code becomes really useful for you.