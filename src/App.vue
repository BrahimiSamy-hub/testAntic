<template>
  <!-- <AppNavbar /> -->
  <Hero />
  <Room />
  <Products />
  <Inspirations />
  <!-- <router-view /> -->
  <Footer />
</template>

<script>
import AppNavbar from '@/components/AppNavbar.vue'
import Hero from '@/views/Hero.vue'
import Room from '@/views/Room.vue'
import Products from '@/views/Products.vue'
import Footer from '@/components/Footer.vue'
import Inspirations from '@/views/Inspirations.vue'
import './App.css'

export default {
  components: { AppNavbar, Hero, Room, Products, Inspirations, Footer },
}
</script>
