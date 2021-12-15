<!DOCTYPE html>
<html>
<head>
<title>About Streetware</title>
<link rel="stylesheet" href="style.css">
<header>
<h1>About Streetware</h1>
<h2>By Joe Sherman- Bsc Cyber Secuirty student at ARU.</h2>
<a href="index.php">Home</a>
<a href="registration.php">Registration</a>
<a href="about.php">About</a>
<div class="image1">
	<iframe src="https://giphy.com/embed/12GA6HQ5bK7kK4" width="100%" height="10%" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/swag-ymcmb-follow-me-12GA6HQ5bK7kK4">via GIPHY</a></p>
</div>
</header>
</head>
<body>
<section>
<h1>Streetwear Database!</h1>
<table>
	<tr>
		<th>id</th>
		<th>Brand name</th>
		<th>Location</th>
		<th>date</th>
	</tr>
	<?php 
	$conn = mysqli_connect("localhost", "root", "", "streetwear");
	$sql = "SELECT * FROM brands";
	$result = $conn-> query($sql);

	if ($result->num_rows > 0) {
		while ($row = $result-> fetch_assoc()) {
			echo "<tr><td>". $row["id"]."</td><td>". $row["Brand name"]."</td><td>". $row["Location"]."</td><td>". $row["date"]."</td></tr>";
		}
			}
	
		else{
			echo "No Results";
		}
	$conn->close();
	?>
	
</table>
<table>
	<tr>
		<th>ID</th>
		<th>Item Name</th>
		<th>Release Date</th>
		<th>Price</th>
	</tr>
	<?php 
	$conn = mysqli_connect("localhost", "root", "", "streetwear");
	$sql = "SELECT * FROM item";
	$result = $conn-> query($sql);

	if ($result->num_rows > 0) {
		while ($row = $result-> fetch_assoc()) {
			echo "<tr><td>". $row["ID"]."</td><td>". $row["Item Name"]."</td><td>". $row["Release Date"]."</td><td>". $row["Price"]."</td></tr>";
		}
			}
	
		else{
			echo "No Results";
		}
	$conn->close();
	?>
	
</table>
</section>
</body>
<footer>
<h4>THIS IS A WEBSITE MADE FOR EDUCATIONAL PURPOSES ONLY! ALL ASSETS USED IN THIS WEBSITE ARE NOT OWNED BY MYSELF. ALL RIGHTS ARE RESERVED TO THE ORIGINAL OWNERS AND RESPECTED COMPANIES. IN ADDITION I WONT BE MAKING ANY COMMERCIAL REVENUE FROM THIS WEBSITE. THANK YOU.</h4>
</footer>
</html>
