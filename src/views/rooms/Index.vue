<template>
  <h1
    style="
      margin-left: 150px;
      margin-top: 64px;
      font-size: 55px;
      font-weight: 400;
      color: #706458;
    "
    data-aos="fade-up"
  >
    Find you room
  </h1>
  <div style="display: flex; margin-left: 150px" data-aos="fade-up">
    <p style="width: 165px">
      Dining room, bedroom, bathroom or office. Find what you need
    </p>
    <swiper
      style="margin-right: 150px"
      :slidesPerView="2"
      :navigation="{
        nextEl: '.custom-next',
        prevEl: '.custom-prev',
      }"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide>
        <h2 class="slide-title">Bedroom</h2>
        <img
          src="../../assets/Picture(1).png"
          loading="lazy"
          alt=""
          class="slide-image"
        />
        <p>dsqds</p>
      </swiper-slide>

      <swiper-slide>
        <h2 class="slide-title">Living room</h2>
        <img
          src="../../assets/Picture(2).png"
          loading="lazy"
          alt=""
          class="slide-image"
        />
        <p>dsqds</p>
      </swiper-slide>

      <swiper-slide>
        <h2 class="slide-title">Bedroom</h2>
        <img
          src="../../assets/Picture(1).png"
          loading="lazy"
          alt=""
          class="slide-image"
        />
        <p>dsqds</p>
      </swiper-slide>

      <swiper-slide>
        <h2 class="slide-title">Living room</h2>
        <img
          src="../../assets/Picture(2).png"
          loading="lazy"
          alt=""
          class="slide-image"
        />
        <p>dsqds</p>
      </swiper-slide>

      <div class="swiper-navigation">
        <span class="custom-next"
          >Next
          <img src="../../assets/Right.svg" alt="" />
        </span>
      </div>
    </swiper>
  </div>
</template>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Pagination, Navigation } from 'swiper/modules'
import 'swiper/css'
import 'swiper/css/pagination'
import 'swiper/css/navigation'

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination, Navigation],
    }
  },
}
</script>

<style>
.custom-next {
  cursor: pointer;
}
.swiper-navigation {
  margin-top: 48px;
  color: #a06056;
  font-size: 20px;
  font-weight: 700;
}
.swiper {
  width: 100%;
  height: 100%;
  margin: 0;
}
.swiper-slide {
  display: flex;
  align-items: center;
}
.slide-title {
  position: absolute;
  color: #a06056;
}
.slide-image {
  object-fit: contain;
}
@media screen and (max-width: 768px) {
}
@media screen and (max-width: 1024px) {
}
</style>
