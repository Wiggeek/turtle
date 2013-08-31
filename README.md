turtle
======
<?php
	$title = "Home";
	$page = 1;
	$path = "";
	
	require "structures/header.php";
?>
		
		<div class="promo-banner clouds" style="background-position: 0px 0px;">
			<div class="clouds"></div>
			<div class="promo-holder">
				<div class="container">
					<div class="row">
						<div class="span7">
							<div class="padding">
								<h1><?=$db->read("Home Page Head");?></h1>
								
								<p><?=$db->read("Home Page Body");?></p>
								
								<button class="btn btn-large" type="button" onclick="window.location='tools.php';"><?=$db->read("Home Page Button Text");?></button>
							</div>
						</div>
						<div class="span5">
							<img src="<?=$db->read('Home Banner 500x300');?>" alt="<?=$db->read('Website Name');?>">
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<div class="features">
			<div class="container">
				<div class="row">
					<div class="span4">
						<div class="feature-icon">
							<img src="<?=$db->read('Column Image 140x140 1');?>" class="img-circle" alt="Brand New Approach">
						</div>
						<div class="feature-content">
							<h2><?=$db->read('Column Title 1');?></h2>
							<p><?=$db->read('Column Text 1');?></p>
						</div>
					</div>
					<div class="span4">
						<div class="feature-icon">
							<img src="<?=$db->read('Column Image 140x140 2');?>" class="img-circle" alt="Feature 2">
						</div>
						<div class="feature-content">
							<h2><?=$db->read('Column Title 2');?></h2>
							<p><?=$db->read('Column Text 2');?></p>
						</div>
					</div>
					<div class="span4">
						<div class="feature-icon">
							<img src="<?=$db->read('Column Image 140x140 3');?>" class="img-circle" alt="Feature 3">
						</div>
						<div class="feature-content">
							<h2><?=$db->read('Column Title 3');?></h2>
							<p><?=$db->read('Column Text 3');?></p>
						</div>
					</div>
				</div>
			</div>
		</div>
		
<?php
	require "structures/footer.php";
?>
