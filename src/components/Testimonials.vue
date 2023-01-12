<template>
    <section id="testimonials">
        <div>
            <h2>Testimonials</h2>
            <NavBar/>
            <center>
                <div class="btn-group p-2" role="group" aria-label="Basic outlined example">
                    <a href="#projects" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-up"></i></a>
                    <a href="#contact" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-down"></i></a>
                  </div>
            </center>
        </div>
        <!-- <div class="container">
        </div> -->
        <!-- <div class="row">
            <div class="card" v-for="item in info" :key="item" style="width: 18rem;">
                <img src="" class="card-img-top" alt="...">
                <div class="card-body">
                  <h5 class="card-title">{{item.name}}</h5>
                  <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
              </div>
        </div> -->
    </section>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
    name: 'Testimonials',
    components: {
        NavBar
    },
    data() {
        return {
            info : [
                {
                    name: 'Brogan',
                    image: "",
                    message: '>Open, chilled guy who you can easily communicate with. Always willing to help regardless if himself is busy. Does not shy away from a challenge. Understands things quicker than most people.'
                },
                {
                    name: 'Imraan',
                    image: "",
                    message: 'Meezaan is a friendly person, he likes to help where he can, always positive and smart with his approach.He is a big football fan and enjoys music. I feel like he will go far in life, whatever he does in the future.'
                },
                {
                    name: 'Mueen',
                    image: "",
                    message: 'Meezaan is a chilled and honest guy.He always gives 100% to anything he faces. He will always be willing to help the next person. He is a goal driven individual. A real "COOL" guy.'
                },
                {
                    name: 'Reece',
                    image: "",
                    message: 'Meezaan is a very ambitious and always gives best, whilst always being ready to assist others.'
                },
                {
                    name: 'Asandile',
                    image: "",
                    message: 'He is a down to earth person, who is always smiling and he is reliable , you can count on him at all time. He is always willing to help people and he does not shy away from showing his soft side. He has a vast awareness of his surroundings and that makes him a focused person.'
                },
                {
                    name: 'test',
                    image: "",
                    message: ''
                }
            ]
        }
    }
}
</script>
<style scoped>
#testimonials {
    height: 100vh;
    background-image: linear-gradient( rgb(216, 191, 191), white);
  }
  .container{
    width: 100%;
    padding: 30px 30px 50px;
    background-color: white;
    border: 2px solid rgba(255,255,255,0.06);
    border-radius: 10px;
    box-shadow: 0 20px 30px rgba(0,0,0,0.2);
    backdrop-filter: blur(10px);
}
</style>