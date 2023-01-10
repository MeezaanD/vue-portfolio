<template>
  
  <section><Home/></section>
  <section><About/></section>
  <Resume/>
  <Projects/>
  <Testimonials/>
  <Contact/>
  <Footer/>
</template>

<script>
// @ is an alias to /src

import Home from '@/components/Home.vue'
import About from '@/components/About.vue'
import Resume from '@/components/Resume.vue'
import Projects from '@/components/Projects.vue'
import Testimonials from '@/components/Testimonials.vue'
import Contact from '@/components/Contact.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'HomeView',
  components: {
   Home, About, Resume, Projects, Testimonials, Contact, Footer
  }
}
</script>
