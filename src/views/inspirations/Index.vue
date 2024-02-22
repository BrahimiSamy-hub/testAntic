<template>
  <div class="container">
    <NewsLetter />
    <Slider />
    <GridInspirations />
  </div>
</template>

<script>
import NewsLetter from '@/views/inspirations/list/NewsLetter.vue'
import Slider from '@/views/inspirations/list/Slider.vue'
import GridInspirations from '@/views/inspirations/list/GridInspirations.vue'
export default { components: { NewsLetter, Slider, GridInspirations } }
</script>

<style scoped>
.slick-slide {
  margin: 0 20px;
}
.container {
  background-color: white;
  padding-left: 150px;
  /* padding-right: 150px; */
}
@media screen and (max-width: 768px) {
  .container {
    padding-left: 32px;
    padding-right: 32px;
  }
}
@media screen and (max-width: 1024) {
  .container {
    padding-left: 70px;
    padding-right: 70px;
  }
}
</style>
