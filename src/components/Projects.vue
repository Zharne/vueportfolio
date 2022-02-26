<template>
<body>
    <div id='projects'>
  			<div class="container" v-if="projects.length">
  				<div v-for = "project in projects" :key="project.id" class="project">
					  <div class="card">
						  <div class="card-image">
							  <img src="project.img" alt="">
						  </div>
						  <div class="card-content">
							  <h3>{{project.title}}</h3>
							  <p>{{project.details}}</p>
						  </div>
						  <button class="custom-btn btn-9">Github</button><br>
						   <button class="custom-btn btn-9">Netlify</button>
					  </div>
    			</div>
  			</div>
  			<!-- <div v-else>
    			<p>Loading projects...</p>
  			</div> -->
    </div>
</body>
</template>

<script>

export default { 
  data() {
    return {
      projects: []
    }
  },
  mounted() {
    fetch('http://localhost:5000/projects')
      .then(res => res.json())
      .then(data => this.projects = data)
      .catch(err => console.log(err.message))
  }
}
  
</script>



<style>
 #projects{
	 width: 100%;
	 /* background-color:rgba(0, 0, 0, 15%); */
	 margin-top: 2rem;
	
}
.project {
	display: flex;
	/* background-color: rgba(0, 0, 0, 15%); */
}
.container {
	position: relative;
	z-index: 1;
	display: flex;
	justify-content: center;
	align-items: center;
	flex-wrap: wrap;
	margin: 40px 0;
}

.container .card {
	position: relative;
	width: 300px;
	height: 400px;
	/* background: rgba(255, 255, 255, 0.05); */
  	background:#111;
	margin: 20px;
	box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
	border-radius: 15px;
	display: flex;
	justify-content: center;
	align-items: center;
	backdrop-filter: blur(10px);
}

.container .card .content {
	position: relative;
	display: flex;
	justify-content: center;
	align-items: center;
	flex-direction: column;
	transition: 0.5s;
}

.container .card:hover .content {
	transform: translateY(-20px);
}

.container .card .content .imgBx {
	position: relative;
	width: 150px;
	height: 150px;
	overflow: hidden;
}

.container .card .content .imgBx img {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	object-fit: cover;
}

.container .card .content .contentBx h3 {
	color: #fff;
	text-transform: uppercase;
	letter-spacing: 2px;
	font-weight: 500;
	font-size: 18px;
	text-align: center;
	margin: 20px 0 10px;
	line-height: 1.1em;
}

.container .card .content .contentBx h3 span {
	font-size: 12px;
	font-weight: 300;
	text-transform: initial;
}

.container .card .sci {
	position: absolute;
	bottom: 50px;
	display: flex;
}

.container .card .sci li {
	list-style: none;
	margin: 0 10px;
	transform: translateY(40px);
	transition: 0.5s;
	opacity: 0;
}

.container .card:hover .sci li {
	transform: translateY(0px);
	opacity: 1;
}

.container .card .sci li a {
	color: #fff;
	font-size: 20px;
}
#about-me{
  background-color: whitesmoke;
  /* padding-bottom: 30px; */
  height: 100vh;
  width: 100%;
}
.container{
    height: 100vh;
    margin-left: 200px;
    /* padding-bottom:30px ; */
}

/* Button */
.frame {
  width: 90%;
  margin: 40px auto;
  text-align: center;
}
button {
  margin: 20px;
}
.custom-btn {
  width: 130px;
  height: 40px;
  color: #fff;
  border-radius: 5px;
  padding: 10px 25px;
  font-family: 'Lato', sans-serif;
  font-weight: 500;
  background: transparent;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  display: inline-block;
   box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
   7px 7px 20px 0px rgba(0,0,0,.1),
   4px 4px 5px 0px rgba(0,0,0,.1);
  outline: none;
}
.btn-9 {
  border: none;
  transition: all 0.3s ease;
  overflow: hidden;
}
.btn-9:after {
  position: absolute;
  content: " ";
  z-index: -1;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
   background-color: #1fd1f9;
background-image: linear-gradient(315deg, #1fd1f9 0%, #b621fe 74%);
  transition: all 0.3s ease;
}
.btn-9:hover {
  background: transparent;
  box-shadow:  4px 4px 6px 0 rgba(255,255,255,.5),
              -4px -4px 6px 0 rgba(116, 125, 136, .2), 
    inset -4px -4px 6px 0 rgba(255,255,255,.5),
    inset 4px 4px 6px 0 rgba(116, 125, 136, .3);
  color: #fff;
}
.btn-9:hover:after {
  -webkit-transform: scale(2) rotate(180deg);
  transform: scale(2) rotate(180deg);
  box-shadow:  4px 4px 6px 0 rgba(255,255,255,.5),
              -4px -4px 6px 0 rgba(116, 125, 136, .2), 
    inset -4px -4px 6px 0 rgba(255,255,255,.5),
    inset 4px 4px 6px 0 rgba(116, 125, 136, .3);
}

</style>