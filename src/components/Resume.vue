<template>
    <section id="resume">
        <div>
            <h2>Resume</h2>
            <NavBar/>
        </div>
    </section>
</template>

<script>
import NavBar from '@/components/NavBar.vue'

export default {
    name: 'Resume',
    components: {
        NavBar
    }
}
</script>

<style>
#resume {
    height: 100vh;
    width: 100%;
  } 
</style>