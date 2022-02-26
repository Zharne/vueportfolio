<template>
  <div class="sidenav">
    <img src="https://i.postimg.cc/ry7cbbcP/depositphotos-346967382-stock-illustration-initial-logo-design-vector-template.jpg" style="border-radius:50%">
  <a href="#home">Home</a>
  <a href="#about-me">About</a>
  <a href="#resume">Resume</a>
  <a href="#projects">Projects</a>
  <a href="#testimonials">Testimonials</a>
  <a href="#contact">Contact</a>
</div>


</template>

<script>
export default {

}
</script>

<style>

body {
  font-family: "Lato", sans-serif;
}

.sidenav {
  height: 100%;
  width: 200px;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: #111;
  overflow-x: hidden;
  padding-top: 50px;
  
  
}

.sidenav a {
  padding: 6px 8px 6px 16px;
  text-decoration: none;
  font-size: 25px;
  color: #818181;
  display: block;
}

.sidenav a:hover {
  color: #f1f1f1;
}

main {
  margin-left: 200px;
  font-size: 28px; 
  padding: 0px 10px;
}

@media screen and (max-width: 450px) {
  .sidenav {
    padding-top: 15px;
    background-color: blue;
    }
  .sidenav a {font-size: 18px;}
}

</style>