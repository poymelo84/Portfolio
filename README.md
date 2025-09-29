<!DOCTYPE html>
<html lang="eng">
	<!--Head-->
	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width" />
		<title>Jaime Melo Portfolio</title>
		<link rel="stylesheet" type="text/css" href="Portfolio.css">
	</head>
	
	<!--Body-->
	<body class="background">
	
		<!--Navbar-->
		<div class="Navbar">
			<a class="active" href="#Home">Home</a>
			<a href="#About">About</a>
			<a href="#GitHub">GitHub</a>
			<a href="#Contact">Contact</a>
		</div>
		
		<!--Breaks inserted to add space between navbar and the first heading-->
				
		<!--Background video-->
		<div id="Home">
			<video autoplay muted loop id="Typing_Video">
				<source src="video.mp4" type="video/mp4">
				<!--Display message if video fails to run-->
				Your browser does not support HTML5 video.
			</video> 
		</div>
		
		<!--Video text-->
		<div class="Video_Text">
			<br>
			<br>
			<h1 class="white-text"> <>Jaime Melo's Portfolio<> </h1>
			<br>
			<strong>
				<p class="center">
					<q>To be or not to be..that will be up to you.
					</q>
					<br> -Anonymous
					<br>
					<br>My name is Jaime Melo and welcome to my portfolio website. On it, I will tell you about my background and experience. 
					<br>
					Feel free to explore and let me know what you think.
					<br>
					<br>Thank you for your time and have a wonderful day!
				</p>
			</strong>
		</div>
		
		<!--About Section-->
		<div class="Row" id="About">
			<!--Left Column-->
			<div class="Column_1">
				<h1>About</h1>
				<p>
					I am an aspiring software developer who is new to coding but enjoys every bit of it! As a family man, I also enjoy sports and just hanging out with the family.
					<br>
					<br>I am currently a student of <a href="https://www.learncodinganywhere.com" target="_blank">The Tech Academy</a>’s Software Developer Boot Camp, and is currently training in the following web and programming languages: HTML, CSS, JavaScript, SQL, C# and more. 
					<br>
					<br>I may be new to the game but rest assured, I have a strong passion for what I do and will get the job done! <a href="#Contact">Contact</a> me for more info.
				</p>
			</div>
		
		<!--Right Column-->
			<div class="Column_2">
				<img src="img_1.jpg" alt="Replace with your own image and description">
			</div>
			<!--Right Column-->
		</div>
		
		<!--Github section-->
		<div class="Row" id="Github">
			<!--Left Column-->
			<div class="Column_2">
				<a href="https://github.com/" target="_blank"><img src="github_1.jpg"></a>
			</div>
			<!--Right Column-->
			<div class="Column_1">
				<h1>Github</h1>
				<p>
					<h4>Check out my coding projects on my Github profile. Click the link below.</h4>
					<br>
					<p class="center"><a href="https://github.com/poymelo84/HTML-and-CSS-Projects" target="_blank">Jaime's coding projects</a></p>
				</p>
					<h2><img src="github_2.webp" alt="404 file not found" class="no-style"></h2>
			</div>
		</div>
		
		<!--Contact section-->
		<div class="Row" id="Contact">
			<!--Contact form, left column-->
			<div class="Column_1 Column_tall">
				<h1>Contact</h1>
				<!--This specifies where and how to send the form data; we are leaving it blank-->
				<form action="" method="POST"> <!--Here we are utilizing a 3rd party service to submit the contact form data, insert 
					your formspree endpoint in the action attribute-->
					<label>Name:</label>
						<input type="text" placeholder="Please enter your name here">
					<label>Email:</label>
						<input type="text" id="Email" name="Email" placeholder="Please enter you email here">
					<label>Message:</label>
						<input type="text" id="Message" name="Message" placeholder="Please write your message here">
						<input type="submit" value="SUBMIT">
				</form>
			</div>
			<!--Contact image, left column-->
			<div class="Column_2 Column_tall">
				<img src="img_2.webp" alt="Contact_Image">
			</div>
		</div>
		
		<!--Footer section-->
		<footer>
			<p>
				<p class="center">&copy Copyright, <a href="https://www.learncodinganywhere.com/" target="_blank">The Tech Academy</a></p>	 
				<img src="img_3.png" alt="404 file not found" class="no-style1">
			</p>
			</footer>
	</body>
</html>
						



/***** GENERAL STYLING -----/
/* Body */
body {
	margin: 0px /* This ensures our site displays all the way to the edge of the browser
	screen */
}

/* Heading 1 elements */
h1 {
	text-transform: uppercase; /* Capitalizing all h1 headings */
	font-family: "Trebuchet MS", Optima; /* Sets the font family of all h1 headings */
	text-align: center; /* Centering all h1 elements */
	margin-top: 2%; /* Adds a small margin above h1 elements */
	color: #1a1a1a;
}

h4 {
	color: #1a1a1a;
	text-align: center;
	font-family: Calibri;
	font-size: 24px;
}
/*Heading 1 element hover effect */
h1:hover {
	filter: grayscale(5%); /* Adds a slightly fray filter to the h1 headings when hovered 	
over */
	transform: scale(1.1); /* When the h1 elements are hovered over, they increase in size
by 1.1 */
	transition: transform 1s; /* This causes the transformation to last 1 second */
}

/*Styling for the portfolio title text */
.white-text {
	color: #5e85f2; /*This is used to change the color of the portfolio title text */
}

/* Paragraph elements */
p {
	font-family: Calibri;
	text-align: justify; /* Justify text within paragraph elements */
	letter-spacing: 1px; /* This expands the text slightly */
	font-size: 22px;
	padding-left: 20px; /* Adds padding to the left of the paragraph element */
	padding-right: 20px; /* Adds padding to the right of the paragraph element */
}

/* Paragraph element hover effect */
p:hover {
	transition: transform 1s; /* This makes the transform effect last 1 second */
		transform: scale(1.01); /*This makes the paragraph increase slightly in size
when hovered over */
}

/* Center class - this applies to all elements with the class "center" */
.center {
	text-align: center; /* This center aligns the text */
}

/* Center class hover effect - This only affects the quote, github link, and footer */
.center:hover {
	transition: transform 2s; /* This makes the transform effect last 2 seconds */
	transform: scale(1.1); /* This makes the elements with class "center" increase in 
	size by 1.1 when hovered over */
}

/* Anchor elements */
a {
	color: blue; /* This ensures all links are blue */
}

/* Quotation elements */
q {
	font-style: italic; /* This makes the quote italicized */
}

/* Image elements */
img {
	filter: grayscale(25%); /* This rids our pictures of 75% of their color */
	border-radius: 8px; /* Gives all images slightly rounded corners */
	max-width: 75%; /* Ensures all images stay within the width of their container */
	height: 300px; /*Sets the height of all images */
	display: block; /*By specifying block display, we can ensure our images are able to
be centered */
	margin-left: auto; /* In combination with "margin-right: auto" this centers all
images */
	margin-right: auto;
}

.no-style {
	width: 200px;
	height: 85px;
}

.no-style:hover {
  box-shadow: 0 0 20px rgba(78, 135, 234, 0.6);
  transition: box-shadow 0.3s ease;
}

.no-style1 {
	float: right;
	position: relative;
	margin-top: -57px;
	width: 50px;
	height: 50px;
}

/* Image element hover effects */
img:hover {
		filter: grayscale(5%); /*Brings back most of the image's color when hovered
over */
	transition: transform 1s; /* Transition lasts 1s */
		transform: scale(1.1); /*Image is increased slightly when hovered over */
}

/* The @media rule is used in media queries to apply different styles for different
media/types of devices */
/* On screens 576px and smaller, the images will be 100px tall and centered vertically in
the column */
@media screen and (max-width: 576px) {
	img {
		height: 100px;
		margin-top: 150px;
	}
}

/* Styling for footer element */
footer {
	padding: 1%; /* This gives the footer padding that is equal to 2% of the width of the
element's area */
	background-color: rgb(192, 192, 190);
}
/***** END OF GENERAL STYLING *****/


/***** NAVBAR STYLING *****/
.Navbar {
	overflow: hidden; /*This ensures that any content that overflows beyond the boundary
of our navbar is not displayed */
	background-color: rgb(46, 42, 42); /* This colors the navbar black */
	position: fixed; /* This keeps the navbar at the top of the screen as we scroll */
	top: 0; /* This ensures that no space is displayed above the navbar */
	width: 100%; /* This makes the navbar span the entire width of the page */
	z-index: 1; /* This ensures other elements don't display over the navbar */
	-webkit-animation: moveNav 5s; /* This applies the moveNav animation below for Safari
4.0 - 8.0 */
	animation: moveNav 5s; /* This applie the moveNav animation for all the other browsers
*/
}

/* moveNav animation effect for moving the nav bar in from the left of the screen */
@keyframes moveNav {
	from {left: -100vw;} /* The navbar is starting off screen to the left */
	to {left: 0vw;} /* This moves the navbar into place on the screen */
}

/* Navbar links */
.Navbar a {
	float: left; /* This specifies that the text floats on the left on the navbar */
	display: block; /* This ensures that other text will be displayed on the same line or
row, instead of a new line */
	color: white; /* This is the font color for text on our navbar */
	padding: 14px 16px; /*This adds padding around our text */
	text-decoration: none; /* This gets rid of the underlines under the text on our
navbar */
	font-family: Avant garde, Helvetica; /* This specifies the font family for text on
our navbar */
	font-size: 20px; /*This specifies the font size for text on our navbar */
	text-align: center; /*This centers the text within its container */
	position: relative; /*This sets the text relative to its normal positioning,
allowing us to use the animation below */
	-webkit-animation: moveNavText 5.75s; /* Animation for Safari 4.0 - 8.0 */
	animation: moveNavText 5,75s; /* Applies the moveNavText animation for 5.75s */
}

/* moveNavText animation effect for moving the navbar text from above the view to the
navbar */
@keyframes moveNavText {
	from {top: -100vw;} /* This sets the navbar text 100% above the viewport */
	to {top: 0vw;} /* This lowers the navbar text onto the navbar */
}

/* Screens 576px and smaller will display navbar links eqully distributed */
@media screen and (max-width: 576px) {
	.Navbar a{
		width: 25%; /* This makes each link take up 1/4 of the navbar */
		font-size: 12px;
	}
}

/* Navbar hover effects */
.Navbar a:hover {
	background-color: #f4f4f4; /*Defines the background color that will display when you hover over the link */
	color: black; /* This defines the font color that will display when navbar elements are hovered over */
	font-weight: bold; /* This makes the text on the navbar bold when hovered over */
}

/* Navbar home button */
.Navbar a.active { /* This targets the a element on the navbar with the "active" class */
		background-color: darkgray;
}
/***** END OF NAVBAR STYLING *****/

/*****VIDEO STYLING *****/
/* Formatting for background video */
#Typing_Video {
	position: fixed; /* This fixes the video to the page */
	right: 0; /* This ensures that there is no space between the edge of the video and the edge of teh page */
	bottom: 0; /* This ensures no space between the bottom of the video and the bottom of the page */
	min-width: 100%; /* This ensures the video is displayed across the full width of the page */
	z-index: -1; /* This places the video behind the other elements on the page */
}

/* Screens that are 576px and smaller will not display the background video */
@media screen and (max-width: 576px) {
	#Typing_Video {
		display: none;
	}
}

/* Texts over the video */
.Video_Text {
	background: rgba(0, 0, 0, 0.5); /* This provides a semi-transparent background for the text to sit over */
	color: white; /* Makes the font color white */
	width: 100%; /* Ensures the video-text container fills the width of the video */
	padding: 20px; /* This adds padding around the video-text container so that the background goes slightly beyond the text */
	position: relative; /* This sets the text relative to its normal positioning, allowing us to use the animation below */
	-webkit-animation: moveVideoText 5.75s;
	animation: moreVideoText 5.75s;
	font: Perpetua;
}

/* This animation effect causes the overlay video text to move up from the bottom of the page upon page load */
@keyframes moveVideoText {
	from {top: -100vw;} /* This sets the position of the video text to above the viewport */
	to {top: 0vw;} /* This moves the video text to the normal positioning on the viewport */
}
/***** END OF VIDEO STYLING *****/

/***** TABLE STYLING - this section covers the styling of the columns and rows within the table *****/
* { /* The asterisk is a universal selector that applies this effect to all elements on the page */
	box-sizing: border-box; /* This creates a box with a border within which we will place most of our text */
}

.Column_1 {
	float: left;
	width: 50%; /* This ensures the column takes up half of the page width */
	padding: 10px;
	padding-top: 1%; /* This ensures there is space between the top of the column and our headings */
	height: 400px; /*This sets the height of the column to 400px - this may need to be adjusted depending on the text you enter */
	background-color: #f2f2f2; /* Sets the background color of the columns with class Column_1 */
}


/*Screens 576px and smaller will display a scroll bar if the text overflows the column height */
@media screen and (max-width: 576px) {
	.Column_1 {
		overflow: auto;
	}
}

.Column_2 {
	float: left;
	width: 50%;
	padding: 10px;
	padding-top: 1.9%;
	height: 400px;
	background-color: #98b0e4
}

/* This class is applied to the columns in the final row, overriding the height and padding to provide more room
for the contact form while keeping the rest of the formatting from Column_1 or Column_2 */
.Column_tall {
	padding-top: 3,5%;
	height: 400px;
}

/* This inserts something after the content of selected elements (in this case, the elements with the class "Row") */
.Row:after {
		content: ""; /* By leaving this blank, we are allowing the footer (covered lower down) to be displayed - removing
		it makes the footer overwrite a column */
		display: table; /*The display property specifies the type of display behavior; the table value tell the browser to 
treat the element as a table */
		clear: both; /* This clears any other elements from floating on the left or the right of an element */
}
	
/**** END OF TABLE STYLING *****/

/***** CONTACT FORM STYLING *****/
/* input[type=text] targets all text input sections of the contact form */
input[type=text] {
	width: 100%; /* Each input box covers the full width of the container */
	padding: 12px; /* Adds padding within the text box */
	border: 1px solid #ccc; /* Setting a solid border and its color */
	border-radius: 4px; /* Slightly rounds the corners of the text box border */
	box-sizing: border-box; /* This creates a box with a border around the contact form input boxes */
	margin-top: 6px; /* Adds a margin to the top of the text box */
	margin-bottom: 16px; /* Adds a margin to the bottom of the text box */
	resize: vertical; /* This allows the user to resize the text boxes vertically */
	font-family: Perpetua, Rockwell Extra Bold;
	font-size: 18px;
}

/* Hover effects for input boxes */
input[type=text]:hover {
	box-shadow: 0 0 5px #00004d inset; /* This creates a blue shadow in the text box when hovered over by the user */
}

/* Submit button */
input[type=submit] {
	background-color: black; /* Sets the background color of the submit button to black */
	color: white; /* Sets the font color of the Submit button to white */
	font-weight: bold; /* Makes the font of the Submit button to bold */
	font-size: 20px;
	padding: 12 px 20 px; /* Adds padding to the submit button */
	border: none; /* Removes the border from the submit button */
	border-radius: 4px; /* Gives the submit button the same rounded corners as the text boxes */
	cursor: pointer; /* Changes the cursor to pointer when over the Submit button */
	display: block; /* Allows the submit button to be centered */
	margin-left: auto; /* In combination with "margin-right: auto", this will center the submit button */
	margin-right: auto;
	font-family: Perpetua, Rockwell Extra Bold;
	margin-top: 1%;
}

/* Hover effect for submit button */
input[type=submit]:hover {
	background-color: white; /* Turns the background of the submit button wite when the user hovers over it */
	color: black; /* Turns the font black when hovered over */
	transform: scale(1.5); /* Makes the button increase 1.5 imes in size */
	transition: transform 1.5s; /* Makes the transform effect last 1.5 seconds */
}

/* Form element */
form {
	border-radius: 5px; /* Rounds the corners of the contact form */
	background-color: #f2f2f2;
	padding: 0px; /* Adds padding to the contact form */
	font-family: "Trebuchet MS", Optima;
}

/***** END OF CONTACT FORM STYLING *****/
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	













































		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
		





