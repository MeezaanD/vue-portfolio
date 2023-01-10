<template>
    <div>
         <button class="btn btn-dark m m-1" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasTop" aria-controls="offcanvasTop">Navigation</button>

            <div class="offcanvas offcanvas-top" tabindex="-1" id="offcanvasTop" aria-labelledby="offcanvasTopLabel">
              <div class="offcanvas-header bg-dark text-light">
                <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
              </div>
              <div class="offcanvas-body bg-dark light">
                <div class="topnav">
                    <a href="#home">Home</a>
                    <a href="#about">About</a>
                    <a href="#resume">Resume</a>
                    <a href="#projects">Projects</a>
                    <a href="#testimonials">Testimonials</a>
                    <a href="#contact">Contact</a>
                  </div>
              </div>
            </div>
    </div>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style>
.topnav a {
    float: left;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    font-size: 25px;
    
  }
  
  .topnav a:hover {
    background-color: #ddd;
    color: black;
  }
</style>