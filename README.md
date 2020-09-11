<!DOCTYPE html>
<html>
<head>
	<title>car</title>
<style>
	.myfav{
		height: 100vh;
		width: 100%;
		background-image: url(sky.jpg);
		background-size: cover;
		background-position: center;
		position: relative;
		overflow-x: hidden;
	}
	.highway{
		height: 200px;
		width: 500%;
		display: block;
		background-image: url(road.jpg);
		position: absolute;
		bottom: 0;
		left: 0;
		right: 0;
		z-index: 1;
		background-repeat: repeat-x;
		animation: highway 10s linear infinite;
	}
	   @keyframes highway
	{
		100%{
			transform: translate(-3400px);
		}
	}
	.city{
		height: 250px;
		width: 500%;
		background-image: url(city.png);
		position: absolute;
		bottom: 200px;
		left: 0;
		right: 0;
		display: block;
		z-index: 1;
		background-repeat: repeat-x;
		animation: city 20s linear infinite;
	}
	@keyframes city
	{
		100%{
			transform: translateX(-1400px);
		}
	}
	.car{
		width: 400px;
		left: 50%;
		bottom: 100px;
		transform: translateX(-50%);
         position: absolute;
         z-index: 2;
	}
	.car img
	{
		width: 100%;
		animation: : car 1s linear infinite;
	}
	@keyframes car: {
		100%{
			transform: translateY(-1px);
		}
		50%{transform: translateY(-1px);
		}
		0%{transform: translateY(-1px);
		}
	}
	.wheel{
		left: 50%;
		bottom:178px;
		transform: translateX(-50%);
		position: absolute;
		z-index: 2;
	}
	.wheel img
	{
		width: 72px;
		height: 72px;
		animation: wheel 1s linear infinite;
	}
	.back-wheel
	{
		left: -165px;
		position: absolute;
	}
	.front-wheel
	{
		left: 80px;
		position: absolute;
	}
	@keyframes wheel
	{
		100%{transform: rotate(360deg);}
	}
</style>
</head>
<body>
	<section><h1>saiteja</h1></section>
	<div class="myfav">
		<div class="highway"></div>
		<div class="city"></div>
		<div class="car">
			<img src="car.png">
		</div>
		<div class="wheel">
			<img src="wheel.png" class="back-wheel">
			<img src="wheel.png" class="front-wheel">
		</div>
</div>

</body>
</html>
