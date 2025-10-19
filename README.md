<!DOCTYPE html>
<html lang="eng">
	<!--Head-->
	<head>
		<meta charset="UTF-8">
		<meta name="viewport" content="width=device-width" />
		<title>Jaime Melo's Portfolio</title>
		<link rel="stylesheet" type="text/css" href="Portfolio.css">
		<script src="Portfolio.js" defer></script>
	</head>

	
	<!--Body-->
	<body class="background">
	
		<!--Navbar-->
		<div class="Navbar">
			<a class="active" href="#Home">Home</a>
			<a href="#Slideshow">Slideshow</a>
			<a href="#About">About</a>
			<a href="#Github">Github</a>
			<!-- Onclick and ondblclick functions added to open and close the contact form -->
            <a onclick="openForm()" ondblclick="closeForm()" class="#contact">Contact</a>
		</div>
		
		<!--Breaks inserted to add space between navbar and the first heading-->
		<br>
		<br>
		
		<!--Background video-->
		<div id="Home">
			<video autoplay muted loop id="Typing_Video">
				<source src="C:\Users\jaime\OneDrive\Documents\GitHub\HTML-and-CSS-Projects\Portfolio\video.mp4" type="video/mp4">
				<!--Display message if video fails to run-->
				Your browser does not support HTML5 video.
			</video> 
		</div>
		
		<!--Video text-->
		<div class="Video_Text">
			<br>
			<br>
			<h1 class="white-text">Jaime Melo's Portfolio</h1>
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

		<!--Slideshow-->

		<div id="Slideshow">
            <div id="Slideshow_Background"> 
                <div id="Slideshow_Container">
                    <!-- Slide 1 of 5 -->
                    <div class="mySlides fade">
                        <img class="Slideshow_Images" src="img_8.jpg" alt="404 file not found">
                        <div class="text">Hello, My name is Jaime and I can help you with your coding needs!</div>
                    </div>
                    <!-- Slide 2 of 5 -->
                    <div class="mySlides fade">
                        <img class="Slideshow_Images" src="img_4.jpg" alt="404 file not found"> 
                        <div class="text">I am a full-stack software developer,<br> currently training in:<br>HTML, CSS, JavaScript,</div>
                    </div>
                    <!-- Slide 3 of 5 -->
                    <div class="mySlides fade">
                        <img class="Slideshow_Images" src="img_5.png" alt="404 file not found">
                        <div class="text">the popular programming language Python,</div>
                    </div>
                    <!-- Slide 4 of 5 -->
                    <div class="mySlides fade">
                        <img class="Slideshow_Images" src="img_6.webp" alt="404 file not found">
                        <div class="text">back end development, databases and SQL.</div>
                    </div>
                    <!-- Slide 5 of 5 -->
                    <div class="mySlides fade">
                        <img class="Slideshow_Images" src="img_7.webp" alt="404 file not found"> 
                        <div class="text">For any inquiries, send me a message and I'll reply ASAP!</div>
                    </div>
                    
                    <!-- Previous and next buttons -->
                    <a class="Previous" onclick="plusSlides(-1)">&#10094;</a>
                    <a class="Next" onclick="plusSlides(1)">&#10095;</a>
                </div>
                <br> <!-- Adds a space between the slideshow images and the dots -->

                <!-- Slideshow dots (these are another way for users to navigate through the slideshow) -->
                <div style="text-align: center">
                    <span class="dot" onclick="currentSlide(1)"></span>
                    <span class="dot" onclick="currentSlide(2)"></span>
                    <span class="dot" onclick="currentSlide(3)"></span> 
                    <span class="dot" onclick="currentSlide(4)"></span> 
                    <span class="dot" onclick="currentSlide(5)"></span> 
                </div>
            </div>
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
				<img src="C:\Users\jaime\OneDrive\Documents\GitHub\HTML-and-CSS-Projects\Portfolio\img_1.jpg" alt="Replace with your own image and description">
			</div>
			<!--Right Column-->
		</div>
		
		<!--Github section-->
		<div class="Row" id="Github">
			<!--Left Column-->
			<div class="Column_2">
				<a href="https://github.com/" target="_blank"><img src="C:\Users\jaime\OneDrive\Documents\GitHub\HTML-and-CSS-Projects\Portfolio\github_1.jpg" alt="GitHub Logo"></a>
			</div>
			<!--Right Column-->
			<div class="Column_1">
				<h1>Github</h1>
				<p>
					<h4>Check out my coding projects in my Github profile. Click the link below.</h4>
					<br>
					<p class="center"><a href="https://github.com/poymelo84" target="_blank">Jaime's coding projects</a></p>
				</p>
					<h2><img src="C:\Users\jaime\OneDrive\Documents\GitHub\HTML-and-CSS-Projects\Portfolio\github_2.webp" alt="404 file not found" class="no-style"></h2>
			</div>
		</div>
		
		<!--Contact section-->

		<div class="Row" id="Contact">

		<button class="open-button" onclick="openForm()">CONTACT</button>

		<div class="form-popup" id="myForm">
  			<form action="/action_page.php" class="form-container">
    		<h1>CONTACT</h1>

    		<label for="namel"><b>Name</b></label>
    		<input type="text" placeholder="Type your name here" name="name" required>

    		<label for="phone"><b>Phone</b></label>
    		<input type="text" placeholder="Type your phone number here" name="phone" required>

			<label for="email"><b>Email</b></label>
    		<input type="text" placeholder="Type your email here" name="email" required>

			<label for="message"><b>Message</b></label>
    		<input type="text" placeholder="Type your message here" name="message" required>

    		<button type="submit" class="btn">Submit</button>
    		<button type="button" class="btn cancel" onclick="closeForm()">Close</button>
  			</form>
		</div>
		
		<!--Footer section-->
		<footer>
			<p>
				<p class="center">&copy Copyright, <a href="https://www.learncodinganywhere.com/" target="_blank">The Tech Academy</a></p>	 
				<img src="C:\Users\jaime\OneDrive\Documents\GitHub\HTML-and-CSS-Projects\Project Folder\images\Thumb\thumbnail_15.png" alt="404 file not found" class="no-style1">
			</p>
			</footer>
	</body>
</html>
						
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			
			

		
