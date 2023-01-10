<template>
  <section id="home"></section>
  <div class="landing-img">
    <center>
      <div class="btn-group" role="group" aria-label="Basic outlined example">
        <a href="#home" class="btn text-light">Home</a>
        <a href="#about" class="btn text-light">About</a>
        <a href="#resume" class="btn text-light">Resume</a>
        <a href="#projects" class="btn text-light">Projects</a>
        <a href="#testimonials" class="btn text-light">Testimonials</a>
        <a href="#contact" class="btn text-light">Contact</a>
      </div>
    </center>
  </div>
  
</template>

<script>
export default {
  name: 'Home',

}
</script>


<style>

#home {
  max-height: 1px;
  width: 100%;
}

.logo {
  position: relative;
  right: 15%;
  height: 400px;
}

.text  {
  color: white;
  margin: 0;
  float: none;
  top: 0%;
  left: 50%;
  position: relative;
}

.text p  {
  font-size: large;
}

.landing-img {

  background-image: url("https://i.postimg.cc/Pqg47HGZ/tech.jpg");
  height: 100vh;
  overflow: hidden;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.container {
  position: absolute;
  margin: 20px;
  width: auto;
}

.topnav {
  overflow: hidden;
  background-color:transparent;
}

.topnav a {
  float: none;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 25px;
  position: relative;
  left: 30%;
  
}

.topnav a:hover {
  background-color: #ddd;
  color: black;
}

*{
  margin: 0;
  padding: 0;
}

#home {
  height: 1px;
}
</style>
