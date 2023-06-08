<?php 
include 'dbconnect.php';
if (isset($_GET['success'])) {

} 
?>

<!DOCTYPE html>
<html>
<head>
	<title>Express Delivery Service</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>

	<section class="main">

	<nav>
		<a href="#" class="logo">
			<img class="zamba" src="images2.jpg">
		</a>

		<ul class="menu">
			<li><a href="#" class="active">Home</a></li>
			<li><a href="#">Login</a></li>
			<li><a href="#">Sign Up</a></li>
			<li><a href="#">Tracking</a></li>
		</ul>
	</nav>

	<div class="main-heading">
		<h1>Express Delivery Service</h1>
		<p>Your delivery is our utmost priority, Delivery is our watchword.</p>
		<a class="main-btn" href="#">Contact</a>
	</div>
	</section><br><br><br>

    <p id="clock" style="width: 300px; height: 60px; font-size: 40; color: #000080; margin-left: 10px; margin-top: -50px; "></p>
    <button onclick="clock()" type="submit" class="main-btn contact-btn" style="width: 150px; margin-left: 10px; margin-top: 10px;">Display Current Time</button>


	<section class="features">
		<div class="feature-container">

			<div class="feature-box">
				<div class="f-img">
					<img src="webicon.jpg">
				</div>
				<div class="f-text">
					<h4>Create Shipment</h4>
					<p>Create your shipment on the go..</p>
					<a href="" class="main-btn">Check</a>
				</div>
			</div>

			<div class="feature-box">
				<div class="f-img">
					<img src="softicon.png">
				</div>
				<div class="f-text">
					<h4>Track Shhipment</h4>
					<p>Track your shipment in real time</p>
					<a href="" class="main-btn">Check</a>
				</div>
			</div>

			<div class="feature-box">
				<div class="f-img">
					<img src="appicon.png">
				</div>
				<div class="f-text">
					<h4>Contact Us</h4>
					<p>24/7 online customer care support</p>
					<a href="" class="main-btn">Check</a>
				</div>
			</div>

		</div>
	</section>

	<section class="about">
		<div class="about-img">
			<img src="images2.jpg">
		</div>
		<div class="about-text">
			<h2>Start Tracking Your Shipment today</h2>
			<p>We are a reputable shipping company that offers comprehensive solutions tailored to the unique needs of our clients, which include manufacturers, distributors, retailers, and individuals..</p>
			<button class="main-btn">Read More</button>
		</div>
	</section>

	<section class="contact">
		<div class="contact-heading">
			<h1>Contact Us</h1>
			<p>Contact us for a reliable and efficient shipping services.</p>
		</div>
		<form method="POST" action="<?php $_SERVER['PHP_SELF']; ?>">
			<input type="text" name="user" placeholder="Your full name">
			<input type="email" name="email" placeholder="Your E-mail">
			<textarea name="message" placeholder="Enter your message here......"></textarea>
			<button type="submit" class="main-btn contact-btn">Continue</button>
		</form>
	</section>

	<?php 
    if ($_SERVER["REQUEST_METHOD"] == "POST") {
    	$user = $_POST['user'];
    	$email = $_POST['email'];
    	$message = $_POST['message'];

    	$sql = "INSERT INTO userinfodata (user,email,message) VALUES ('$user','$email','$message')";

    	if (mysqli_query($connect, $sql)) {
    		header("location: index.php?success");
    	} else {
    		echo "Registration failed! " . $sql. "<br>" .mysqli_error($connect);
    	}

    	mysqli_close($connect);
    }
	?>
   
<script src="index.js"></script>
</body>
</html>
