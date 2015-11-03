# Smooth Navigational Menu #

*Description:* Smooth Navigation Menu is a multi level, CSS list based menu powered using jQuery that makes website navigation a smooth affair. And that's a good thing given the important role of this element in any site. The menu's contents can either be from direct markup on the page, or an external file and fetched via Ajax instead. And thanks to jQuery, a configurable, sleek "slide plus fade in" transition is applied during the unveiling of the sub menus. The menu supports both the horizontal and vertical (sidebar) orientation.

## Directions ##

*Step 1:* This script uses the following external files:

+ jQuery 1.4 or above (served via Google CDN)
+ ddsmoothmenu.js
+ ddsmoothmenu.css
+ ddsmoothmenu-v.css
+ 4 images

*Step 2:* Add the below code to the HEAD section of your page:

	<!DOCTYPE html>
	
	<link rel="stylesheet" type="text/css" href="ddsmoothmenu.css" />
	<link rel="stylesheet" type="text/css" href="ddsmoothmenu-v.css" />
	
	<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.8/jquery.min.js"></script>
	<script type="text/javascript" src="ddsmoothmenu.js">
	
	/***********************************************
	* Smooth Navigational Menu- (c) Dynamic Drive DHTML code library (www.dynamicdrive.com)
	* Please keep this notice intact
	* Visit Dynamic Drive at http://www.dynamicdrive.com/ for full source code
	***********************************************/
	
	</script>
	
	<script type="text/javascript">
	
	ddsmoothmenu.init({
		mainmenuid: "smoothmenu1", //menu DIV id
		orientation: 'h', //Horizontal or vertical menu: Set to "h" or "v"
		classname: 'ddsmoothmenu', //class added to menu's outer DIV
		//customtheme: ["#1c5a80", "#18374a"],
		contentsource: "markup" //"markup" or ["container_id", "path_to_menu_file"]
	})
	
	ddsmoothmenu.init({
		mainmenuid: "smoothmenu2", //Menu DIV id
		orientation: 'v', //Horizontal or vertical menu: Set to "h" or "v"
		classname: 'ddsmoothmenu-v', //class added to menu's outer DIV
		method: 'toggle', // set to 'hover' (default) or 'toggle'
		arrowswap: true, // enable rollover effect on menu arrow images?
		//customtheme: ["#804000", "#482400"],
		contentsource: "markup" //"markup" or ["container_id", "path_to_menu_file"]
	})
	
	</script>

*Step 3:* Then, add the below sample markup to your page:

	<!-- Markup for mobile menu toggler. Hidden by default, only shown when in mobile menu mode -->
	<a class="animateddrawer" id="ddsmoothmenu-mobiletoggle" href="#">
	<span></span>
	</a>
	
	<h2>Example 1</h2>
	
	<div id="smoothmenu1" class="ddsmoothmenu">
	<ul>
	<li><a href="http://www.dynamicdrive.com">Item 1</a></li>
	<li><a href="http://www.dynamicdrive.com">Folder 0</a>
	  <ul>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.1</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  </ul>
	</li>
	<li><a href="http://www.dynamicdrive.com">Folder 1</a>
	  <ul>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.1</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  </ul>
	</li>
	<li><a href="http://www.dynamicdrive.com">Item 3</a></li>
	<li><a href="http://www.dynamicdrive.com">Folder 2</a>
	  <ul>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 2.1</a></li>
	  <li><a href="http://www.dynamicdrive.com">Folder 2.1</a>
	    <ul>
	    <li><a href="http://www.dynamicdrive.com">Sub Item 2.1.1</a></li>
	    <li><a href="http://www.dynamicdrive.com">Sub Item 2.1.2</a></li>
	    <li><a href="http://www.dynamicdrive.com">Folder 3.1.1</a>
			<ul>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.1</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.2</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.3</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.4</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.5</a></li>
			</ul>
	    </li>
	    <li><a href="http://www.dynamicdrive.com">Sub Item 2.1.4</a></li>
	    </ul>
	  </li>
	  </ul>
	</li>
	<li><a href="http://www.dynamicdrive.com/style/">Item 4</a></li>
	</ul>
	<br style="clear: left" />
	</div>
	
	
	<h2 style="margin-top:200px">Example 2</h2>
	
	<div id="smoothmenu2" class="ddsmoothmenu-v">
	<ul>
	<li><a href="http://www.dynamicdrive.com">Item 1</a></li>
	<li><a href="http://www.dynamicdrive.com">Folder 0</a>
	  <ul>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.1</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  </ul>
	</li>
	<li><a href="http://www.dynamicdrive.com">Folder 1</a>
	  <ul>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.1</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.2</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.3</a></li>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 1.4</a></li>
	  </ul>
	</li>
	<li><a href="http://www.dynamicdrive.com">Item 3</a></li>
	<li><a href="http://www.dynamicdrive.com">Folder 2</a>
	  <ul>
	  <li><a href="http://www.dynamicdrive.com">Sub Item 2.1</a></li>
	  <li><a href="http://www.dynamicdrive.com">Folder 2.1</a>
	    <ul>
	    <li><a href="http://www.dynamicdrive.com">Sub Item 2.1.1</a></li>
	    <li><a href="http://www.dynamicdrive.com">Sub Item 2.1.2</a></li>
	    <li><a href="http://www.dynamicdrive.com">Folder 3.1.1</a>
			<ul>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.1</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.2</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.3</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.4</a></li>
	    		<li><a href="http://www.dynamicdrive.com">Sub Item 3.1.1.5</a></li>
			</ul>
	    </li>
	    <li><a href="http://www.dynamicdrive.com">Sub Item 2.1.4</a></li>
	    </ul>
	  </li>
	  </ul>
	</li>
	<li><a href="http://www.dynamicdrive.com/style/">Item 4</a></li>
	</ul>
	<br style="clear: left" />
	</div>

## Smooth Navigational Menu set up ##

See script project page for additional details on setup and documentation: <http://www.dynamicdrive.com/dynamicindex1/ddsmoothmenu.htm>
