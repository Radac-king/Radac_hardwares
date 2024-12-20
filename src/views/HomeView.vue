<script setup>
import Navbar from '@/components/NavbarComponent.vue'
import Hero from '@/views/HeroView.vue'
import About from '@/views/AboutView.vue'
import service from '@/views/ServiceView.vue'
import Work from '@/views/MyworkView.vue'
import Contact from '@/views/ContactView.vue'
import Footer from '@/components/FooterComponent.vue'

</script>

<template>
  <Navbar/>

  <section class="hero_content" id="Hero">
    <Hero/>
  </section>

  <section class="main_container" id="About">
    <About/>
  </section>

  <section class="main_container" id="Service">
    <service/>
  </section>

  <section class="main_container" id="Work">
    <Work/>
  </section>

  <section class="main_container" id="Contact">
    <Contact/>
  </section>

  <section class="footer_content" id="Footer">
    <Footer/>
  </section>
  
</template>
