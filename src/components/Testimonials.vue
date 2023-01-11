<template>
    <section id="testimonials">
        <div>
            <h2>Testimonials</h2>
            <NavBar/>
        </div>
        <!-- <div class="container">
        </div> -->
    </section>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
    name: 'Testimonials',
    components: {
        NavBar
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