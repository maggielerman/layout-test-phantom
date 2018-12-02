---
layout: post
title:  "Maggie's test post!"
date:   2016-07-18 12:00:00 -0400
categories: jekyll update
---
$base-duration: 500ms;
<style>
// Colors
$color-1: #c0392b;
$color-2: #5A7D7C;
$color-3: #e74c3c;

// Breakpoints
$sm: new-breakpoint(min-width 320px);
$med: new-breakpoint(min-width 768px);
$lg: new-breakpoint(min-width 1024px);

*, *:before, *:after {
    box-sizing: border-box;
    outline: none;
}


.hide { opacity: 0; }

body {
    font-family: 'Source Sans Pro', sans-serif;
    font-size: 16px;
    font-smooth: auto;
    font-weight: 300;
    line-height: 1.5;
    color: #444;
}

.container {
    position: relative;
    display: block;
    width: 80%;
    height: 100%;
    margin: 0 auto;
}

header {
    position: relative;
    display: block;
// align-items: center;
// justify-content: center;
    width: 100%;
    height: 90vh;
    margin: 0;
    padding: 20px 0 0;
    overflow: hidden;
    z-index: 0;

&:before, &:after {
               position: absolute;
               content: '';
               top: 0;
               left: 0;
               width: 100%;
               height: 100%;
           }

&:before {
     background-color: rgba($color-3,0.8);
     z-index: 0;
 }

&:after {
     filter: blur(5px);
     background-attachment: fixed;
     background-image: url('https://static.pexels.com/photos/266526/pexels-photo-266526.jpeg');
     background-position: bottom center;
     background-repeat: no-repeat;
     background-size: cover;
     animation: blur 10s linear infinite;
     overflow: hidden;
     z-index: -1;

@keyframes blur {
    0%   { filter: blur(1px); }
    50%  { filter: blur(20px); }
    100% { filter: blur(1px); }
}
}

nav {
    position: relative;
    z-index: 2;

.logo {
    position: relative;
    display: inline-block;
    width: 50px;
    height: 50px;
    margin: 0;
    border-radius: 50%;

svg {
    position: absolute;
    transform: scale(1);
    animation: scale $base-duration * 1.5 ease-in-out;
}

@keyframes scale {
    0%   { transform: scale(100);
        opacity: 0; }
    50%  { transform: scale(0.2); }
    70%  { transform: scale(1); }
    90%  { transform: scale(0.7); }
    100% { transform: scale(1);
        opacity: 1; }
}
}

.subscribe {
    position: relative;
    display: inline-block;
    padding: 15px 0;
    float: right;
    animation: slide $base-duration * 2 ease;

a {
    position: relative;
    margin: 0;
    padding: 10px 20px;
    background-color: white;
    border-radius: 4px;
    box-shadow: 0 0 35px rgba(black,0.3);
    color: $color-3;
    font-size: 13px;
    text-decoration: none;
    text-transform: uppercase;
    transition: box-shadow 500ms ease;

&:hover {
     box-shadow: 0 0 0 rgba(black,0.0);
 }
}

@keyframes slide {
    0%   { transform: translateY(-600px);
        opacity: 0; }
    100% { transform: translateY(0px);
        opacity: 1; }
}
}
}

blockquote {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 90%;
    margin: 0;
    padding: 5px 0 5px 30px;
// border-left: 5px solid white;
    color: white;
    font-size: 24px;
    font-weight: 100;
    line-height: 1.25;
    letter-spacing: 2px;
    transform: translate(-50%,-50%);
    animation: fadeIn $base-duration * 2.5 ease;

&:before {
     position: absolute;
     content: '';
     top: 0;
     left: 0;
     width: 5px;
     height: 100%;
     background-color: white;
     animation: height $base-duration * 2 ease-in-out;

@keyframes height {
    0%   { height: 0; }
    100% { height: 100%; }
}
}

@keyframes fadeIn {
    0%   {
        opacity: 0;
        transform: translate(-50%,-150%);
    }

    100% {
        opacity: 1;
        transform: translateY(-50%,0%);
    }
}

// 		@include media($med) {
// 			width: 70%;
// 		}

// 		@include media($lg) {
// 			width: 60%;
// 		}

span {
    position: relative;
    display: block;
    margin: 20px 0 0;
    font-size: 16px;
}
}

.date {
    position: absolute;
    bottom: 20px;
    margin: 0;
    padding: 5px 15px;
    border: 2px solid white;
    border-radius: 4px;
    color: white;
    font-size: 12px;
    font-weight: 400;

i {
    margin-right: 5px;
    font-size: 14px;
}
}
}

section {
    position: relative;
    display: block;
    margin: 0;
    padding: 100px 0;
    z-index: 999;

.scroll {
    position: absolute;
    right: 50px;
    top: -20px;
    width: 40px;
    height: 40px;
    background-color: white;
    border-radius: 50%;
//box-shadow: 0 0 25px rgba(black,0.3);

i {
    position: relative;
    top: 50%;
    left: 50%;
    color: $color-3;
    transform: translate(-50%,-100%);
    animation: down 2s ease infinite;
    z-index: 9;

@keyframes down {
    100% {
        transform: translate(-50%,-30%);
        opacity: 0;
    }
}
}
}

.container {
    width: 80%;

// 		@include media($med) {
// 			width: 70%;
// 		}

// 		@include media($lg) {
// 			width: 50%;
// 		}
}

h1 {
    margin: 0;
    padding: 0;
    color: $color-2;
    line-height: 1.5;
}

.byline {
    position: relative;
    display: block;
    width: 100%;
    margin-bottom: 50px;
    font-style: italic;
    vertical-align: middle;

.avatar {
    position: relative;
    display: inline-block;
    top: 10px;
    width: 30px;
    height: 30px;
    margin-right: 5px;
    background-image: url('https://images-na.ssl-images-amazon.com/images/M/MV5BMTQ2NjM5NjE5NF5BMl5BanBnXkFtZTYwNTk3MjUz._V1_UY317_CR0,0,214,317_AL_.jpg');
    background-size: cover;
    background-color: $color-2;
    border-radius: 50%;
}

span {
    color: $color-3;
    font-style: normal;
    font-weight: bold;
}
}

p {
    margin-bottom: 50px;
    font-family: 'Merriweather',serif;
    font-size: 16px;
    line-height: 1.95;

.drop {
    position: relative;
    display: inline-block;
    margin: 0 20px 0 0;
    color: $color-3;
    font-size: 64px;
    font-weight: bold;
    line-height: 1.2;
    float: left;
}
}

blockquote {
    position: relative;
    width: 80%;
    margin: 150px auto;
    padding: 5px 0 5px 30px;
    border-left: 5px solid $color-3;
    color: #444;
    font-size: 20px;
    line-height: 1.75;

span {
    position: relative;
    display: block;
    margin: 20px 0 0;
    font-size: 16px;
}
}
}

.quote {
    height: 400px;
    background-attachment: fixed;
    background-position: center center;
    background-repeat: no-repeat;
    background-size: cover;
    overflow: hidden;

&.desert {
     background-image: url('https://static.pexels.com/photos/80454/tree-desert-namibia-dead-vlei-80454.jpeg');
 }

&.second {
     background-image: url('https://static.pexels.com/photos/36464/sky-clouds-clouds-form-cumulus-clouds.jpg');
 }

&:before {
     position: absolute;
     content: '';
     top: 0;
     left: 0;
     width: 130%;
     height: 100%;
     background-color: rgba(white,0.8);
     box-shadow: inset 0 0 30px rgba(black,0.3);
     z-index: -1;
 }

blockquote {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 44%;
    margin: 0;
    padding: 5px 0 5px 30px;
    border-left: 5px solid $color-3;
    color: #444;
    font-size: 24px;
    font-weight: 100;
    line-height: 1.25;
    letter-spacing: 2px;
    transform: translate(-50%,-50%);

span {
    position: relative;
    display: block;
    margin: 20px 0 0;
    font-size: 16px;
}
}
}

.comments {
    padding-top: 0;

.toggle {
    position: relative;
    display: block;
    width: 100%;
    margin: 10px 0 50px;
    padding: 10px;
    background-color: lighten($color-2,10%);
    border-radius: 4px;
    box-shadow: 0 0 20px rgba(black,0.3);
    color: white;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;

.indicator {
    position: relative;
    top: 4px;
    width: 15px;
    height: 16px;
    line-height: 1.75;
    transition: transform 250ms ease;
    float: right;

&:before, &:after {
               position: absolute;
               content: '';
           }

&:before {
     top: 50%;
     width: 100%;
     height: 2px;
     background-color: white;
     transform: translateY(-1px);
 }

&:after {
     left: 50%;
     width: 2px;
     height: 100%;
     background-color: white;
     transform: translateX(-1px);
 }
}
}

#toggle {
    display: none;

&:checked + .toggle {

.indicator {
    transform: rotate(45deg);
}
}

&:checked ~ .wrapper {
     height: auto;
 }
}

.wrapper {
    position: relative;
    display: block;
    height: 0;
    overflow: hidden;

.comment {
    position: relative;
    display: flex;

.user {
    position: relative;
    width: 80px;
    height: inherit;
    margin: 0 20px 20px 0;
    padding: 0;
    float: left;
    font-size: 12px;
    text-align: center;

.pic {
    position: relative;
    width: 100%;
    height: 65px;
    margin: 6px auto;
    background-image: url('http://images.complex.com/complex/image/upload/c_limit,w_680/fl_lossy,pg_1,q_auto/Screen_Shot_2015-09-08_at_12.11.35_PM_sy22b5.jpg');
    background-position: center center;
    background-size: cover;
    background-color: darkgray;
    overflow: hidden;
}

.date {
    font-size: 12px;
}
}

.text {

.author {
    font-weight: bold;
    text-transform: uppercase;
    color: $color-3;
}

p {
    position: relative;
    margin: 0;
    padding: 0;
    font-size: 14px;
}
}
}
}
}

.tags {
    position: relative;
    display: block;
    margin: 0;
    padding: 0;
    list-style-type: none;

li {
    position: relative;
    display: inline-block;
    margin: 0 5px 5px 0;

&.tag {
     display: block;
     color: $color-3;
     font-weight: bold;
     text-transform: uppercase;
 }

a {
    position: relative;
    display: block;
    padding: 7px 20px;
    background-color: $color-2;
    border-radius: 99px;
    color: white;
    font-size: 12px;
    font-weight: bold;
    text-transform: uppercase;
    text-decoration: none;

&:hover {
     background-color: lighten($color-2,10%);
 }
}
}
}




// footer
   .footer {
       position: relative;
       display: block;
       width: 100%;
       margin: 0;
       padding: 50px 0 0;
       background: $color-1;
       z-index: 0;

.footer-logo {
    position: relative;
    display: block;
    width: 50px;
    height: 50px;
    margin: 0 auto;
    background-color: white;
    border-radius: 50%;
}

.footer-links {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-bottom: 20px;
}

ul {
    flex-basis: 13em;
    flex-shrink: 0;
    margin-bottom: 40px;
    padding: 0;

li {
    line-height: 1.5em;
    list-style: none;
    text-align: center;

a {
    color: transparentize(white,0.5);
    text-decoration: none;

&:focus,
&:hover {
     color: transparentize(white,0);
 }
}

h3 {
    color: white;
    font-size: 1em;
    margin-bottom: 0.4em;
}
}
}

.disclaimer {
    position: relative;
    display: block;
    width: 100%;
    padding: 30px;
    background-color: darken($color-1,10%);

p {
    color: transparentize(white,0.4);
    font-size: 12px;
    font-weight: 400;
    line-height: 1.5;
    margin: auto;
    max-width: 35%;
    text-align: center;
}
}
}
</style>
<header>
	<div class="container">
		<nav>
			<div class="logo">
				<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
					 viewBox="0 0 50 50" style="enable-background:new 0 0 50 50;" xml:space="preserve">
					<style type="text/css">
						.st0{fill:#FFFFFF;}
						.st1{fill:#B93D30;}
					</style>
					<circle class="st0" cx="25" cy="25" r="25"/>
					<g>
						<polygon class="st1" points="34.1,25 27.7,13.9 21.3,25 19.2,28.7 16.5,24 13,30 9.5,36.1 14.9,36.1 16.5,36.1 23.5,36.1 
													 27.7,36.1 40.5,36.1 	"/>
					</g>
				</svg>
			</div>
			<div class="subscribe">
				<a href="#">Subscribe</a>
			</div>
		</nav>
		<blockquote>The magic Indian is a mysterious spiritual force, and we're going to Cathedral Rock, and that's the vortex of the heart.
		<span>&mdash; Gary Busey</span>
		</blockquote>
		<div class="date">
			<i class="fa fa-calendar" aria-hidden="true"></i> 
			August 1, 2017
		</div>
	</div>
</header>

<section>
	<div class="scroll">
		<i class="fa fa-long-arrow-down" aria-hidden="true"></i>
	</div>
	<div class="container">
		<h1>I wrestled a bear once. 750lbs.</h1>
		<div class="byline">
			<div class="avatar"></div>
			by <span>Gary Busey</span>
		</div>
		<p class="hide"><span class="drop">Y</span>ou gotta go through it to see there ain't nothing to it. Did you feel that? Look at me - I'm not out of breath anymore! Go with the feeling of the nature. Take it easy. Know why you're here. And remember to balance your internal energy with the environment. </p>

		<p class="hide">Listen to the silence. And when the silence is deafening, you're in the center of your own universe. It's OK to get Rib-grease on your face, because you're allowing people to see that you're proud of these ribs. The best way to communicate is compatible. Compatible communication is listening with open ears and an open mind, and not being fearful or judgemental about what you're hearing.</p>
	</div>
</section>

<section class="quote desert">
	<blockquote>These kind of things only happen for the first time once.</blockquote>
</section>

<section>
	<div class="container">
		<p class="hide">The best way to communicate is compatible. Compatible communication is listening with open ears and an open mind, and not being fearful or judgemental about what you're hearing. Go with the feeling of the nature. Take it easy. Know why you're here. And remember to balance your internal energy with the environment. These kind of things only happen for the first time once.You ever roasted doughnuts?The best way to communicate is compatible. Compatible communication is listening with open ears and an open mind, and not being fearful or judgemental about what you're hearing.</p>

		<p class="hide">The best way to communicate is compatible. Compatible communication is listening with open ears and an open mind, and not being fearful or judgemental about what you're hearing. Have you urinated? Have you drained your bladder? Are you free? Because if you haven't it will only come out later. I'm giving you some information that your bodily fluids may penetrate your clothing fibre's without warning.</p>
		
		<!-- <blockquote class="hide">
			Sometimes horses cough and fart at the same time, so stay out of the range of its butt muscle because a horses butt muscle is thick. <span>&mdash; Gary Busey</span>
		</blockquote> -->

		<p class="hide">The magic Indian is a mysterious spiritual force, and we're going to Cathedral Rock, and that's the vortex of the heart.When you get lost in your imaginatory vagueness, your foresight will become a nimble vagrant.I wrestled a bear once. A 750lbs black bear.</p>
	</div>
</section>


<section class="quote second">
	<blockquote>I would like to give you a backstage pass to my imagination.</blockquote>
</section>

<section>
	<div class="container">
		<p class="hide">Sometimes horses cough and fart at the same time, so stay out of the range of its butt muscle because a horses butt muscle is thick.When you get lost in your imaginatory vagueness, your foresight will become a nimble vagrant. The best way to communicate is compatible. Compatible communication is listening with open ears and an open mind, and not being fearful or judgemental about what you're hearing.</p>
		
		<p><strong>FIN!</strong></p>
		
		<ul class="tags">
			<li class="tag">Tags</li>
			<li><a href="#">Psychedelic</a></li>
			<li><a href="#">Spiritual</a></li>
			<li><a href="#">WTF</a></li>
			<li><a href="#">Gary Busey</a></li>
			<li><a href="#">Philosophy</a></li>
			<li><a href="#">Deep Thoughts</a></li>
			<li><a href="#">Drugs</a></li>
			<li><a href="#">Doctrine</a></li>
		</ul>
	</div>
</section>

<section class="comments">
	<div class="container">
		<input type="checkbox" id="toggle" />
		<label class="toggle" for="toggle">
			Toggle Comments <i class="indicator"></i>
		</label>
		<div class="wrapper">
			
			<!-- COMMENT -->
			<div class="comment">
				<div class="user">
					<div class="pic"></div>
					<div class="date">06/16/2017</div>
				</div>
				
				<div class="text">
					<div class="author">Joaquin Phoenix</div>
					<p>Thats an advanced modern oxymoron. It was good, I like it and I beleived it. Man you got a way with using words. Thats like a lariat that does a snake whip on your back legs, I mean on the back of your legs - not that you have 4 legs - and pulls you this way, and thats what that line did to me and I believed every minute of it. Until I looked at the quadrangle that it produced with the verbs used in the sentence.</p>
				</div>
			</div>
		</div>
	</div>
</section>
	
<footer class="footer">
	<div class="footer-logo">
		<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
			 viewBox="0 0 50 50" style="enable-background:new 0 0 50 50;" xml:space="preserve">
			<style type="text/css">
				.st0{fill:#FFFFFF;}
				.st1{fill:#B93D30;}
			</style>
			<circle class="st0" cx="25" cy="25" r="25"/>
			<g>
				<polygon class="st1" points="34.1,25 27.7,13.9 21.3,25 19.2,28.7 16.5,24 13,30 9.5,36.1 14.9,36.1 16.5,36.1 23.5,36.1 
											 27.7,36.1 40.5,36.1 	"/>
			</g>
		</svg>
	</div>
	<div class="footer-links">
		<ul>
			<li><h3>Content</h3></li>
			<li><a href="#">About</a></li>
			<li><a href="#">Contact</a></li>
			<li><a href="#">Products</a></li>
		</ul>
		<ul>
			<li><h3>Follow Us</h3></li>
			<li><a href="#">Facebook</a></li>
			<li><a href="#">Twitter</a></li>
			<li><a href="#">YouTube</a></li>
		</ul>
		<ul>
			<li><h3>Legal</h3></li>
			<li><a href="#">Terms &amp; Conditions</a></li>
			<li><a href="#">Privacy Policy</a></li>
		</ul>
	</div>

	<div class="disclaimer">
		<p>Copyright &copy; <script>document.write(new Date().getFullYear());</script> &nbsp;&nbsp;|&nbsp;&nbsp; Magic Indian Spiritual Mysteries, LLC</p>
	</div>
</footer>
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes.