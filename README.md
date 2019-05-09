Read me 

This is a compilation of a README created for the used template and my own additons. 

---------------------------
Part one / Template Read me (original creator)

Big Picture by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)


This is Big Picture, a simple, single page responsive site template by HTML5 UP.

So I've been on a single page kick as of late, partly because I'm lazy, but
mostly because they kick ass for experimentation. In this case, Big Picture
makes heavy use of my (tentatively named and soon to be released) "scrollgress"
and "scrollwatch" jQuery plugins to pull off some interesting effects as you
scroll around the page. In addition to said interesting effects, Big Picture
also includes a nice lightbox-style gallery, styling for basic page elements,
and thoroughly commented code for your editing pleasure (with instructions!
-- see below).

Many thanks to my good friends Felicia Simion (ineedchemicalx.deviantart.com)
and Michael Domaradzki (md.photomerchant.net) for allowing me to use their amazing
photos in Big Picture's demo*.

(* = Not included! Only meant for use with my own on-site demo, so please do NOT
download and/or use any of Felicia's or Michael's work without their explicit
permission!)

AJ
aj@lkn.io | @ajlkn

PS: Not sure how to get that contact form working? Give formspree.io a try (it's awesome).


Instructions:

	Overview:

		Being a single pager, Big Picture should be way simpler to work with than
		some of the heavier stuff I've released in the past. In fact, aside from
		a main page <header> and <footer>, it's pretty much just a stack of "main"
		<section> elements that follow the same basic pattern:

			<section id="foobar" class="main">
				<div class="content container">
					<header>
						<h2>Foobar</h2>
					</header>
					...
				</div>
			</section>

		The section can then be assigned a style class to determine its basic
		look (and, in some cases, its behavior):

			style1
				Centered content with an oversized <h2>. Works best when
				paired with a background image or color.

			style2 left
				Content in a box, anchored to the left side of the window. Works
				best when paired with a background image or color. If you have
				"useSectionTransitions" turned on in your settings, the box will
				slide into view from the left.

			style2 right
				Content in a box, anchored to the right side of the window. Works
				best when paired with a background image or color. If you have
				"useSectionTransitions" turned on in your settings, the box will
				slide into view from the right.

			style3 primary
				Used for generic content. Set against the primary background
				color (default is white).

			style3 secondary
				Used for generic content. Set against the secondary background
				color (default is a light gray).

		Oh, and there are a few (well, two) optional modifier classes you can
		tack on for additional effects:

			dark
				Flips the content's color scheme so it shows up better
				against darker background images and colors.

			fullscreen
				Makes the section fill the entire window (only if "useFullScreen"
				is enabled in your settings).


	Lightbox Gallery:

 		The actual gallery function is powered by my Poptrox plugin. For info on
 		how that works, go here: github.com/ajlkn/jquery.poptrox

		Each image (the '...' bit in the above examples) should look like this:

			<article class="from-(direction)">
				<a href="path/to/fullsize.jpg" class="image fit">
					<img src="path/to/thumbnail.jpg" title="This is the image caption." alt="" />
				</a>
			</article>

		The "from-(direction)" class indicates the direction from which the image should
		slide into view, and can be any of the following:

			from-left
			from-right
			from-bottom
			from-left

		You can also just remove the "from-(direction)" class if you don't want that particular
		image to slide into view (in which case it'll simply fade in).


	Contact Form:

		To get this working, place a script on your server to receive the form data, then
		point the "action" attribute to it (eg. action="http://mydomain.tld/mail.php").
		More on how it all works here: 1stwebdesigner.com/tutorials/custom-php-contact-forms


    Icons:

     	Powered by Font Awesome. Go here for a full listing of all the icons you can use:
     	fontawesome.io


	Other Stuff:

		- If you don't like the way images are tinted, either change "images/overlay.png"
		  to something else, or remove all references to it from css/style.css.


Credits:

	Demo Images:
		Felicia Simion (ineedchemicalx.deviantart.com)
			"The Swallow Song"
			"Mind is a clear stage"
			"The Anonymous Red"
			"The sparkling shell"
			"Carry on"

		Michael Domaradzki (md.photomerchant.net)
			"Vine Country"
			"Airchitecture II"
			"Bent IX"
			"Air Lounge"

	Icons:
		Font Awesome (fontawesome.io)

	Other:
		jQuery (jquery.com)
		Poptrox (github.com/ajlkn/jquery.poptrox)
		Scrollex (github.com/ajlkn/jquery.scrollex)
		Responsive Tools (github.com/ajlkn/responsive-tools)

----------------------------
Part two / READ ME ADDITIONS

First of all I would like to credit AJ, the maker of this template. It is thanks to his hard work that I could whip out a decent looking webpage in just a few hours. All credit for the layout and more belongs to them. 

As you can see and read this is an extremely easy template to use and adapt. 



INSTALLATION

The template is easy to use, all you have to do is download the directory and open it via your IDE and just start to adjust and adapt it to your own desires. 



LICENSE

If you look closely to my Github repo you'll see the original license, provided by the creator themselves. Check it out if you need to. 


CHANGELOG

9th of May 2019

This template has been adapted to my own requirement.  I have added my own images and changed the colors, icons and repurposed some of the sections. I have also changed the color of the form beacuse it was lacking visibility and needed a little enhancement. Just like the font. The colorscheme was inoffensive but made it lightly unreadble, especially when used on a device with a smaller screen. 


USER EXPERIENCE

It is basically a one pager that consists of multiple image boxes hence making it faily easy to use and to implement as long as you keep in mind to make sure you use the correct path. 

Most of the layout is divided in sections that are easy to manage and to rename according to your preference. 

The Sass directory contains all the scss-files, referring to the sections, icons etc... So if you are not sure where something is, just checkout you html code and look up the reference.

All the colors can be found in the libs/_vars map/file for a good overview, just make sure you double check the var names and you'll be able to change the colorscheme of the entire page. You can look up the variable by checking out the typography.scss.


Pay attention to the form, it might me to light to be visible so make changes accordingly.

BUGS

When implementing my own gallery I had some problems with the path to my images. For some reason creating a path to the directories images/fulls was not working and I had to use a roundabout way to make sure my images were being displayed. I just moved the images used in the gallery and put them in the main directory, that way no filepath was required. 

