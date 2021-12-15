<!DOCTYPE html>
<html>
<head>
<title>Joe's Uni Website</title>
<link rel="stylesheet" href="style.css">
<header>
<h1>Welcome to my website!</h1>
<h2>By Joe Sherman- Bsc Cyber Secuirty student at ARU.</h2>
<a href="registration.php">Registration</a>
<a href="about.php">About</a>
<a href="Streetweardatabase.php">Database</a>
<div class="image1">
	<iframe src="https://giphy.com/embed/12GA6HQ5bK7kK4" width="100%" height="10%" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/swag-ymcmb-follow-me-12GA6HQ5bK7kK4">via GIPHY</a></p>
</div>
</header>
</head>
<body>
<section>
<h1>Streetwear and clothing!</h1>
<p>This website will cover information on various streetwear and clothing brands. Of which, I will include a databse containing various information on these said brands.</p>
<p> Also, as seen down below. This website will also contain a database that has information based on various different streetware brands.</p>
<h3>User login form</h3>
<form action="login.php" method="post">
	<table>
		<tr>
			<td>Username:</td>
			<td>
				<input type="text" name="user">
			</td>
		</tr>

		<tr>
			<td>Password:</td>
			<td>
				<input type="password" name="user_pass">
			</td>
		</tr>
		<tr>
			<td>
				<input type="submit" name="submit" value="login">
			</td>
			<td>
				<p>Dont have an account?</p><a href="registration.html">Register</a>
			</td>
		</tr>


	</table>



</form>
<?php
echo "This is my first PHP Script!";
?>


<div class="image2"><img src="off-white-logo.png" alt="Off white logo" height="20%" width="20%">
</div>
<div class="image3"><img src="Bape-Logo.png" alt="A bathing ape logo" height="20%" width="20%">
</div>
<div class="image4"><img src="Supreme-Logo.png"alt="Supreme box logo" height="20%" width="20%">
</section>
</body>
<footer>
<h4>THIS IS A WEBSITE MADE FOR EDUCATIONAL PURPOSES ONLY! ALL ASSETS USED IN THIS WEBSITE ARE NOT OWNED BY MYSELF. ALL RIGHTS ARE RESERVED TO THE ORIGINAL OWNERS AND RESPECTED COMPANIES. IN ADDITION I WONT BE MAKING ANY COMMERCIAL REVENUE FROM THIS WEBSITE. THANK YOU.</h4>
</footer>
</html>
