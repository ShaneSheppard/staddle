#Boilerplate v1.5

A brilliant less boilerplate for small and large scale websites.

##Features

* Flexibility - all of the built in modules are independent, so if you don't use one you can uncomment it
* Responsive grid
* Supports ie7 + (ie7 support will be dropped when clients stop demanding it)
* Easy user configuration
* Css3 mixins
* Css debugging
* Follows [SMACSS](http://smacss.com/)

#Documentation

##Getting Started

* Set your site variables in assets/less/variables.less
* Add your custom modules to the assets/less/modules folder and import them in main.less
* Tell your less compiler to compile main.less to assets/css/main.css
* Use index.html as a template for your html
* Build a cool site:-)

##Customising

Although Boilerplate does come with some in built modules and styles, it is all about customisation.

All of the main setup (e.g. base font size) and module variables are set in assets/less/variables.less.

	// TYPOGRAPHY
	// ----------------------------------------------------

	@TYPE-FontSize: 				16;
	@TYPE-LineHeight: 				24;

Any custom modules (for example a special box) should be placed in the modules folder (assets/less/modules) and imported in main.less (assets/less/main.less) in the modules section. 

	// MODULES
	// ----------------------------------------------------

	@import "modules/special-box.less";

As all of the built in modules are independent (assets/less/lib/modules) you can safely uncomment them in the boilerplate import (assets/less/lib/boilerplate.less) if you don't use them or you want to write your own module.

##Debugging

Boilerplate has css debugging built in to outline any problems with images, links, empty elements and deprecated elements.

To enable debugging simply set the variable @DEBUG to true in assets/less/variables.less.

	// DEBUG
	// ----------------------------------------------------

	@DEBUG:							true;

##Grid

Boilerplate has a very standard grid system. For example if you wanted content to span 12 columns, you would write:

	<div class="grid">
		<div class="span-12">
			<!-- 12 COLUMN CONTENT HERE -->
		</div>
	</div>