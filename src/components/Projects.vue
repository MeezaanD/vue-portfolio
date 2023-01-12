<template>
  <section id="projects">
      <div> 
          <NavBar/>
          <center>
            <div class="btn-group p-2" role="group" aria-label="Basic outlined example">
                <a href="#resume" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-up"></i></a>
                <a href="#testimonials" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-down"></i></a>
              </div>
          </center>
      </div>
      <h2>Projects</h2>
      <h4>My Projects have thus far consisted of HTML, CSS, Javascript</h4>
      <div class="row">
        <div class="card" v-for="item in projects" :key="item" style="width: 25rem;height:25rem;margin:auto;background-color:transparent;">
            <img :src=item.image class="card-img-top" style="width: 100%;height:15rem;padding:20px;" alt="...">
            <div class="card-body">
              <center>
              <h5 class="card-title">{{item.language}}</h5>
              <h6>{{item.name}}</h6>
                <div class="btn-group" role="group" aria-label="Basic outlined example">
                <a :href="item.github" target="_blank" type="button" class="btn btn-outline-dark"><i class="fa-brands fa-github"></i></a>
                <a :href="item.live" target="_blank" type="button" class="btn btn-outline-dark"><i class="fa-brands fa-chrome"></i></a>
               </div>
              </center>
            </div>
          </div>
    </div>
  </section>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
  name: 'Projects',
  components: {
      NavBar
  },
  data() {
      return {
   projects : [
  {
      language: 'HTML & CSS',
      name: 'Portfolio',
      image:"https://i.postimg.cc/mDwG2M4Q/first-Porfolio.png",
      github: "https://github.com/MeezaanD/Portfolio.git",
      live: "https://phenomenal-semolina-67d782.netlify.app/"
  },
  {
      language: 'HTML & CSS',
      name: 'Grid Activity',
      image: "https://i.postimg.cc/x1tvpfRn/grid.png" ,
      github: "https://github.com/MeezaanD/Grid-Activity.git",
      live: "https://gridactivitymeezaan.netlify.app/"
  },
  {
      language: 'HTML & CSS',
      name: 'Ecommerce Website',
      image:"https://i.postimg.cc/rpR1kCSP/ecommerce.png",
      github: "https://github.com/MeezaanD/Ecommerce-Project.git",
      live: "https://ecomprojectmeezaan.netlify.app/"
  },
  {
      language: 'HTML, CSS, Javascript',
      name: 'Point of Sales',
      image: "https://i.postimg.cc/L5YYzyhk/pos.png",
      github: "https://github.com/MeezaanD/MD-POS.git",
      live: "https://meezaanpointofsales.netlify.app"
    },
    {
      language: 'HTML, CSS, Javascript',
      name: 'Calculator App',
      image: "https://i.postimg.cc/4y5DrRMV/calculator.png",
      github: "https://github.com/MeezaanD/Calculator-TEST-.git",
      live: "https://calculator-md240503.netlify.app"
    },
    {
      language: 'Vue',
      name: 'Mini-Project',
      image: "https://i.postimg.cc/prPWhHn1/mini.png",
      github: "https://github.com/MeezaanD/Mini-Project.git",
      live: "https://miniprojectmeezaan.netlify.app/"
    }
], 
  }
  },
}
</script>
<style scoped>
#projects {
  height: 100%;
  background-image: linear-gradient(white, rgb(216, 191, 191));
  width: 100%;
}

h4 {
  text-align: center;
  padding-bottom: 30px;
}

h3 {
  text-align: center;
  padding-top: 20px;
}
.card button:hover {
  opacity: 0.7;
}

</style>