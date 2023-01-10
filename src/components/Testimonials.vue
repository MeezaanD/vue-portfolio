<template>
    <section id="testimonials">
        <div>
            <h2>Testimonials</h2>
            <NavBar/>
        </div>
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

<style>
#testimonials {
    height: 100vh;
    background-color: aqua;
  }
</style>