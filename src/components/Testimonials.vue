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
        <div class="row">
            <div class="flip-card" v-for="item in info" :key="item" style="height: 25rem;width:25rem;margin:auto">
                <div class="flip-card-inner">
                  <div class="flip-card-front">
                    <h5>{{item.name}}</h5> 
                    <img :src="item.image" alt="Avatar" style="width:20rem;height:20rem;">
                  </div>
                  <div class="flip-card-back">
                    <h6>Message</h6>
                    <p>"{{item.message}}"</p>
                  </div>
                </div>
              </div>
        </div>
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
                    name: 'Brogan Gys',
                    image: "https://i.postimg.cc/Ss0d9Wpj/t2.jpg",
                    message: 'Open, chilled guy who you can easily communicate with. Always willing to help regardless if himself is busy. Does not shy away from a challenge. Understands things quicker than most people.'
                },
                {
                    name: 'Imraan Bernksen',
                    image: "https://i.postimg.cc/T3h9Mgd5/t0.jpg",
                    message: 'Meezaan is a friendly person, he likes to help where he can, always positive and smart with his approach.He is a big football fan and enjoys music. I feel like he will go far in life, whatever he does in the future.'
                },
                {
                    name: 'Cassidy Lawrence',
                    image: "https://i.postimg.cc/c4pj7tZd/images.png",
                    message: 'Meezaan is a driven person. He will always make an effort to find a solution and will never hesitate to ask for assistance when necessary. He is a brilliant, intelligent guy who is always willing to give sound advise to anyone who requests it. He also has excellent social skills that make him a wonderful team member. His artistic side nearly never lets him down. He completes tasks once he sets his mind to them.'
                },
                {
                    name: 'Mueen Slamat',
                    image: "https://i.postimg.cc/bv2dkDQB/mueen.jpg",
                    message: 'Meezaan is a chilled and honest guy.He always gives 100% to anything he faces. He will always be willing to help the next person. He is a goal driven individual. A real "COOL" guy.'
                },
                {
                    name: 'Reece Simons',
                    image: "https://i.postimg.cc/R0s5SX6r/reece.jpg",
                    message: 'Meezaan is a very ambitious and always gives best, whilst always being ready to assist others.'
                },
                {
                    name: 'Asandile Langeni',
                    image: "https://i.postimg.cc/kMLxcD7K/Asandile.jpg",
                    message: 'He is a down to earth person, who is always smiling and he is reliable , you can count on him at all time. He is always willing to help people and he does not shy away from showing his soft side. He has a vast awareness of his surroundings and that makes him a focused person.'
                }          
            ]
        }
    }
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@300&display=swap');
#testimonials {
    height: 100%;
    background-image: linear-gradient( rgb(216, 191, 191), white);
    width: 100%;
  }

 h6, p {
    padding: 20px;
  }

  h5 {
    padding: 10px;
    font-family: 'Quicksand', sans-serif;
  }
.flip-card {
    background-color: transparent;
    width: 300px;
    height: 300px;
    perspective: 1000px;
  }
  
  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.6s;
    transform-style: preserve-3d;
    box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  }
  
  .flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
  }
  
  .flip-card-front, .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
  }
  
  .flip-card-front {
    background-color:transparent;
    color: black;
    border-radius: 3px;
  }
  
  .flip-card-back {
    background-color:transparent;
    color: black;
    transform: rotateY(180deg);
  }
</style>