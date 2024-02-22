<template>
  <div style="padding-right: 0" data-aos="fade-up" data-aos-duration="1500">
    <swiper
      :navigation="{
        nextEl: '.custom-next',
        prevEl: '.custom-prev',
      }"
      :breakpoints="breakpoints"
      :pagination="pagination"
      :modules="modules"
      class="mySwiper"
      data-aos="fade-up"
      data-aos-duration="1500"
    >
      <swiper-slide class="slide-image" style="width: 450px; height: 550px">
        <img src="../../../assets/Picture(3).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="width: 450px; height: 550px">
        <img src="../../../assets/Picture(4).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="width: 450px; height: 550px">
        <img src="../../../assets/Picture(4).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="width: 450px; height: 550px">
        <img src="../../../assets/Picture(4).png" alt="" />
      </swiper-slide>
      <h2>Inspirations</h2>
      <p>
        Our experts are keen to stay on top of trends in order to offer you new
        inspirations for your interior and exterior every day. Remember that to
        inspire you we have to inspire ourselves and we want to share that with
        you.
      </p>
      <div
        class="swiper-navigation"
        style="display: flex; flex-direction: row; gap: 11px"
      >
        <span class="custom-prev"
          ><img src="../../../assets/Button.svg" alt="" />
        </span>
        <span class="custom-next"
          ><img src="../../../assets/Button(1).svg" alt="" />
        </span>
        <span style="">pagination</span>
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
      breakpoints: {
        768: {
          slidesPerView: 2.5,
          spaceBetween: 30,
        },
      },
    }
  },
}
</script>

<style scoped>
.custom-next {
  cursor: pointer;
}
.custom-prev {
  cursor: pointer;
}
.swiper-navigation {
  margin-top: 48px;
  color: #a06056;
  font-size: 20px;
  font-weight: 700;
}

.slide-image {
  object-fit: contain;
}
@media screen and (max-width: 768px) {
}
@media screen and (max-width: 1024px) {
}
</style>
