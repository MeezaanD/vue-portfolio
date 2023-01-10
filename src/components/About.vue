<template>
    <div id="about">
    <NavBar/>
    <body>
        <div>
            <div class="wrapper">
                <div class="text-box">
                    <img src="https://i.postimg.cc/Jn84rpSg/images.png" alt="">
                    
                    <h2>About Me</h2>
                    <p>Hello, my name is Meezaan Davids I am 19 years old, and I was born in Cape Town South Africa. I would like to think I am a genuine straight forward person. I am very interested in learning new skills, whether it is cooking or coding I am very much interested in it. I would also like to consider myself a very passionate sports fan. I try to keep up to date with all my sports. I am really interested in a possible career in web design. At this point in my life I am very into learning new things because new experiences bring new opportunities.</p>
                    <div class="col">
                        <h3>Profile</h3>
                        <ul>
                            <li><b>FullName:</b>  Meezaan Davids</li>
                            <li><b>D.O.B:</b> 24/05/03</li>
                            <li><b>Gender:</b> Male</li>
                            <li><b>Citizenship:</b> South African</li>
                        </ul>
                      </div>
                      <div class="btn-group">
                        <a href="#" class="btn btn-dark">Download CV</a>
                        <a href="#contact" class="btn btn-dark">Want to know more</a>
                      </div>

                </div>
            </div>
        </div>
    </body>
    </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue'

export default {
    name: 'About',
    components: {
        NavBar
    }
}
</script>

<style scoped>
#about {
    min-height: 100vh;
    width: 100%;
  } 

  body {
    display: flex;
    justify-content: center;
    align-items: center;
    align-items: center;

  }

  img {
    max-width: 500px;
    height: 450px;
    float: left;
    margin-right: 20px;
    width: 100%;
  }

  .wrapper {
    margin: 150px auto;
    width: 90%;
  }

  li {
    list-style: none;
  }
</style>