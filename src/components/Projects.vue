<template>
    <section id="projects">
        <div>
            <h2>Projects</h2>
            <NavBar/>
        </div>
        <!-- <div class="row h-25">
              <div class="card h-100 w-25" v-for="item in arr" :key="item">
                  <img :src="item.image" style="width: 100%;height:10rem">
                  <h4>{{item.product}}</h4> 
                  <h5>{{item.studio}}</h5>
                  <p>{{item.github}}</p>
                  <button class="btn" v-on:click="showAlert">Purchase</button> 
              </div>
         </div> -->
         <h3>HTML & CSS orientated projects</h3>
         <!-- <div class="row">
            <div class="col-sm-4 mb-3 mb-sm-0 gap p-5">
              <div class="card" v-for="item in arr" :key="item">
                <div class="card-body">
                <img src="item.image" style="width: 100%;">
                  <h5 class="card-title">{{item.language}}</h5>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
              </div>
            </div> -->
            <!-- <div class="col-sm-4  mb-3 mb-sm-0 gap-3 p-5">
              <div class="card">
                <div class="card-body">
                  <h5 class="card-title">Special title treatment</h5>
                  <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
              </div>
            </div>
            <div class="col-sm-4 gap-3 p-5">
              <div class="card">
                <div class="card-body">
                  <h5 class="card-title">Special title treatment</h5>
                  <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                  <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
              </div>
            </div> -->
          <!-- </div> -->
          <div class="card p-5" v-for="item in arr" :key="item">
            <img :src="item.image" style="width: 100%;">
            <h4>{{item.name}}</h4>
            <p>{{item.language}}</p>
            
            <p><button>Github</button><button>Live</button></p>
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
     arr : [
    {
        language: 'HTML & CSS',
        name: 'portfolio',
        image:"https://i.postimg.cc/L5YYzyhk/pos.png",
        studio: "DC",
        github: 'R100',
        live: ''    
    },
    {
        language: 'HTML & CSS',
        name: 'Portfolio',
        image:"https://i.postimg.cc/mDwG2M4Q/first-Porfolio.png",
        studio: "Marvel",
        github: 'R100',
        live: ''    
    },
    {
        language: 'HTML & CSS',
        name: 'Ecommerce',
        image:"https://i.postimg.cc/rpR1kCSP/ecommerce.png",
        studio: "DC",
        github: 'R100',
        live: ''    
    },
] 
    }
    }
}
</script>
<style scoped>
#projects {
    height: 180vh;
    background-image: linear-gradient(white, rgb(216, 191, 191));
    width: 100%;
  }

  h3 {
    text-align: center;
    padding-top: 20px;
  }

  .card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    max-width: 300px;
    margin: auto;
    text-align: center;
    font-family: arial;
    display: flex;
    height: 40vh;
    padding: 10px;
  }
  
  
  .card button {
    border: none;
    outline: 0;
    padding: 10px;
    color: white;
    background-color: #000;
    text-align: center;
    cursor: pointer;
    height: 3rem;
    font-size: 18px;
  }
  
  .card button:hover {
    opacity: 0.7;
  }

</style>