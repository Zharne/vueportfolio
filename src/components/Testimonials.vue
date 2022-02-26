<template>
<section>
<div id='testimonials'>
	<div class="row">
		<div class="col">
			<h2>Testimonials</h2>
			<div id="myCarousel" class="carousel slide" data-ride="carousel">
				<!-- Carousel indicators -->
				<ol class="carousel-indicators">
					<li data-target="#myCarousel" data-slide-to="0" class="active"></li>
					<li data-target="#myCarousel" data-slide-to="1"></li>
					<li data-target="#myCarousel" data-slide-to="2"></li>
                    <li data-target="#myCarousel" data-slide-to="3"></li>
                    <li data-target="#myCarousel" data-slide-to="4"></li>
                    <li data-target="#myCarousel" data-slide-to="5"></li>
				</ol>   
				<!-- Wrapper for carousel items -->
				<div class="carousel-inner">
					<div class="carousel-item active"><br>
						<div class="img-box"><img src="https://i.postimg.cc/Nfzq0qRB/Alex.jpg" alt=""></div>
						<p class="testimonial"></p>
						<p class="overview"><b>Alex Sexwale</b>,Life Choices lecturer</p>
					</div>
					<div class="carousel-item">
						<div class="img-box"><img src="https://i.postimg.cc/Znxr3DNc/Kyle3.jpg" alt=""></div>
						<p class="testimonial">Zharne is a dedicated,hard-working individual striving for greatness</p>
						<p class="overview"><b>Kyle McBryne</b>, Colleague at Life Choices</p>
					</div>
					<div class="carousel-item">
						<div class="img-box"><img src="https://i.postimg.cc/XJ8JgM2p/Amaarah3.jpg" alt=""></div>
						<p class="testimonial">Zharne is a very hard-working individual. She is willing to help others and she is a good team member. Her personality will be a great asset to any work envornment.</p>
						<p class="overview"><b>Amaarah January</b>, Colleague at Life Choices</p>
					</div>
                    <div class="carousel-item">
						<div class="img-box"><img src="https://i.postimg.cc/NMgGFJgY/Bongani3.jpg" alt=""></div>
						<p class="testimonial">Vestibulum</p>
						<p class="overview"><b>Bongani M</b>, Colleague at Life Choices</p>
					</div>
                    <div class="carousel-item">
						<div class="img-box"><img src="https://i.postimg.cc/CLBMx8wd/hannah.jpg" alt=""></div>
						<p class="testimonial">Zharne is a hardworking team player, any team would be lucky to have her on board.</p>
						<p class="overview"><b>Hannah Dalwai</b>, Colleague at Life Choices</p>
					</div>
                    <div class="carousel-item">
						<div class="img-box"><img src="https://i.postimg.cc/RFsCtxrZ/pexels-andrea-piacquadio-3892920.jpg" alt=""></div>
						<p class="testimonial">Vestibulum </p>
						<p class="overview"><b>Mugammad Breda</b>, Colleague at Life Choices</p>
					</div>
				</div>
				<!-- Carousel controls -->
				<a class="carousel-control-prev" href="#myCarousel" data-slide="prev">
					<i class="fa fa-angle-left"></i>
				</a>
				<a class="carousel-control-next" href="#myCarousel" data-slide="next">
					<i class="fa fa-angle-right"></i>
				</a>
			</div>
		</div>
	</div>
</div>
</section>
</template>

<script>
export default {

}
</script>

<style scoped>
section{
	height: 100vh;
}
#testimonials{
	width: 80%;
	background-color: rgb(10, 5, 5);
	margin-left: 180px;
	margin-top: 300px;

} 
.carousel-indicators{
	bottom: 0;
}
.container{
    margin-left: 100px;
	
} 
.container-xl{
    margin-top: 20vh;
	margin-left: 400px;
}
h2 {
	color: #333;
	text-align: center;
	text-transform: uppercase;
	font-family: "Roboto", sans-serif;
	font-weight: bold;
	position: relative;
	margin: 30px 0 60px;
}
h2::after {
	content: "";
	width: 100px;
	position: absolute;
	margin: 0 auto;
	height: 3px;
	background: #8fbc54;
	left: 0;
	right: 0;
	bottom: -10px;
}
.col-center {
	margin: 0 auto;
	float: none !important;
}
.carousel {
	padding: 0 70px;
}
.carousel .carousel-item {
	color: #999;
	font-size: 14px;
	text-align: center;
	overflow: hidden;
	min-height: 290px;
}
.carousel .carousel-item .img-box {
	width: 135px;
	height: 135px;
	margin: 0 auto;
	padding: 5px;
	border: 1px solid #ddd;
	border-radius: 50%;
}
.carousel .img-box img {
	width: 100%;
	height: 100%;
	display: block;
	border-radius: 50%;
}
.carousel .testimonial {
	padding: 30px 0 10px;
}
.carousel .overview {	
	font-style: italic;
}
.carousel .overview b {
	text-transform: uppercase;
	color: #7AA641;
}
.carousel-control-prev, .carousel-control-next {
	width: 40px;
	height: 40px;
	margin-top: -20px;
	top: 50%;
	background: none;
}
.carousel-control-prev i, .carousel-control-next i {
	font-size: 68px;
	line-height: 42px;
	position: absolute;
	display: inline-block;
	color: rgba(0, 0, 0, 0.8);
	text-shadow: 0 3px 3px #e6e6e6, 0 0 0 #000;
}
/* .carousel-indicators {
	bottom: -5px;
} */
.carousel-indicators li, .carousel-indicators li.active {
	width: 12px;
	height: 12px;
	margin: 1px 3px;
	border-radius: 50%;
	border: none;
}
.carousel-indicators li {	
	background: #7AA641;
	border-color: transparent;
	box-shadow: inset 0 2px 1px rgba(0,0,0,0.2);
}
.carousel-indicators li.active {	
	background: #555;		
	box-shadow: inset 0 2px 1px rgba(0,0,0,0.2);
}
</style>