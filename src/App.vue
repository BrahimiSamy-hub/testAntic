<template>
  <AppNavbar />
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
export default {
  components: { AppNavbar, Hero, Room, Products, Inspirations, Footer },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Varta:wght@300..700&display=swap');
#app {
  font-family: 'Varta', sans-serif;
}
li {
  list-style: none;
}
h2 {
  color: #706458;
  font-family: 'Merriweather', serif;
  font-size: 55px;
  font-weight: 400;
}
a {
  text-decoration: none;
}
body {
  background-color: #f3eee8;
  /* margin-left: 90px; */
}
* {
  margin: 0;
  padding: 0;
}
@media screen and (max-width: 768px) {
  h2 {
    font-size: 35px;
  }
}
</style>
