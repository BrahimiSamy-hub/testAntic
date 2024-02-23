<template>
  <div class="container">
    <NewsLetter />
    <Slider class="desktop" />
    <GridInspirations class="mobile" />
  </div>
</template>

<script>
import NewsLetter from '@/views/inspirations/list/NewsLetter.vue'
import Slider from '@/views/inspirations/list/Slider.vue'
import GridInspirations from '@/views/inspirations/list/GridInspirations.vue'
export default { components: { NewsLetter, Slider, GridInspirations } }
</script>

<style scoped>
.desktop {
  display: block;
}
.mobile {
  display: none;
}

.slick-slide {
  margin: 0 20px;
}
.container {
  background-color: white;
}
@media screen and (max-width: 768px) {
  .desktop {
    display: none;
  }
  .mobile {
    display: block;
  }
}
</style>
