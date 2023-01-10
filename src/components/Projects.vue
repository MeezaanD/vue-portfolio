<template>
    <section id="projects">
        <div>
            <h2>Projects</h2>
            <NavBar/>
        </div>
    </section>
</template>

<script>
import NavBar from '@/components/NavBar.vue'

export default {
    name: 'Projects',
    components: {
        NavBar
    }
}
</script>

<style>
#projects {
    height: 100vh;
    background-color: red;
    width: 100%;
  }   
</style>