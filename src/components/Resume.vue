resume
<template>
    <body>
    <section id="resume">
        <div>
            <NavBar/>
            <center>
                <div class="btn-group p-2" role="group" aria-label="Basic outlined example">
                <a href="#about" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-up"></i></a>
                <a href="#projects" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-down"></i></a>
              </div>
            </center>
    <div class="wrapper">
        <div class="shape-1"></div>
        <div class="shape-2"></div>
        <div class="container">
            <h2>My Coding Skills</h2>
            <div class="skills">
                <div class="details">
                    <span>HTML</span>
                    <span>75%</span>
                </div>
                <div class="bar">
                    <div id="html-bar"></div>
                </div>
            </div>
            <div class="skills">
                <div class="details">
                    <span>CSS</span>
                    <span>70%</span>
                </div>
                <div class="bar">
                    <div id="css-bar"></div>
                </div>
            </div>
            <div class="skills">
                <div class="details">
                    <span>Javascript</span>
                    <span>50%</span>
                </div>
                <div class="bar">
                    <div id="js-bar"></div>
                </div>
            </div>
            <div class="skills">
                <div class="details">
                    <span>Bootstrap</span>
                    <span>70%</span>
                </div>
                <div class="bar">
                    <div id="bootstrap"></div>
                </div>
            </div>
            <div class="skills">
                <div class="details">
                    <span>Vue JS</span>
                    <span>40%</span>
                </div>
                <div class="bar">
                    <div id="vue-js"></div>
                </div>
            </div>
        </div>
    </div>
  <div class="container my-5 border border-2 border-light p-5">
  <div id="words">
    <div class="row">
        <h5 style="margin-left: 1.2rem;">Timeline thus far</h5>
      <div class="col-md-6 offset-md-3" v-for="item in resume" :key="item">
        <ul class="timeline-3">
          <li>
            <p><b>{{item.institution}}</b> ({{item.year}})</p>
            <p class="mt-2 text-dark">{{item.description}}</p>
          </li>
        </ul>
      </div>
    </div>
  </div>
  </div>
</div>
</section>
</body>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
    name: 'Resume',
    components: {
        NavBar
    },
    data() {
        return {
            resume : [
                {
                    institution: "Highschool",
                    description: "Graduated from South Peninsula High School 2021.Passed Matric with bachelors",
                    year: "2017-2021",
                },
                {
                    institution: "IT course",
                    description: "Done a software developer course part time on IT Academy",
                    year: "March 2022 - current"
                },
                {
                    institution: "Life Choice Academy",
                    description: "Currently a student at Life Choices Academy",
                    year: "September - current"
                }
            ]
        }
    }
}
</script>
<style scoped>
#resume {
    height: 170vh;
    width: 100%;
    background-image: linear-gradient( rgb(216, 191, 191), white);
  }
.container{
    width: 100%;
    padding: 30px 30px 50px;
    background-color: transparent;
    border: 2px solid rgba(255,255,255,0.06);
    border-radius: 10px;
    box-shadow: 0 20px 30px rgba(0,0,0,0.2);
    backdrop-filter: blur(10px);
}
.container2 {
    width: 100%;
    padding: 30px 30px 50px;
    background-color: transparent;
    border: 2px solid rgba(255,255,255,0.06);
    border-radius: 10px;
    box-shadow: 0 20px 30px rgba(0,0,0,0.2);
    backdrop-filter: blur(10px);
}
@media (max-width: 550px) {
    .container {
        scale:0.6;
    }
}
@media (max-width: 400px) {
    .container {
        scale:0.5;
    }
}
@media (max-width: 300px) {
    .container {
        scale:0.4;
    }
}
@media (max-width: 250px) {
    .container {
        scale:0.3;
    }
}
@media (max-width: 100px) {
    .container {
        scale:0.2;
    }
}
#words {
  color: black;
}
h5 {
    text-align: center;
}
ul.timeline-3 {
  list-style-type: none;
  position: relative;
}
ul.timeline-3:before {
  content: " ";
  background: #D4D9DF;
  display: inline-block;
  position: absolute;
  left: 29px;
  width: 2px;
  height: 100%;
  z-index: 400;
}
ul.timeline-3 > li {
  margin: 20px 0;
  padding-left: 20px;
}
ul.timeline-3 > li:before {
  content: " ";
  background: white;
  display: inline-block;
  position: absolute;
  border-radius: 50%;
  border: 3px solid black;
  left: 20px;
  width: 20px;
  height: 20px;
  z-index: 400;
}
.container *{
    font-family: "Poppins",sans-serif;
    color: black;
    font-weight: 500;
}
h2{
    margin-bottom: 50px;
    letter-spacing: 2px;
    text-align: center;
    font-size: 33px;
    font-weight: bold;
}
.skills:not(:last-child){
    margin-bottom: 30px;
}
.details{
    width: 100%;
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
}
.bar{
    position: relative;
    border: 2px solid transparent;
    border-radius: 20px;
}
.bar div{
    position: relative;
    width: 0;
    height: 9px;
    border-radius: 10px;
    background-color: black;
}
#html-bar{
    animation: html-fill 2s forwards;
}
@keyframes html-fill{
    100%{
        width: 75%;
    }
}
#css-bar{
    animation: css-fill 2s forwards;
}
@keyframes css-fill{
    100%{
        width: 70%;
    }
}
#js-bar{
    animation: js-fill 2s forwards;
}
@keyframes js-fill {
    100%{
        width: 50%;
    }
}
#bootstrap{
    animation: bootstrap-fill 2s forwards;
}
@keyframes bootstrap-fill{
    100%{
        width: 70%;
    }
}
#vue-js{
    animation: vue-js-fill 2s forwards;
}
@keyframes vue-js-fill{
    100%{
        width: 40%;
    }
}
</style>