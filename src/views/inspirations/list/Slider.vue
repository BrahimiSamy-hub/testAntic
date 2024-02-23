<template>
  <div style="">
    <swiper
      :navigation="{
        nextEl: '.custom-next',
        prevEl: '.custom-prev',
      }"
      :slidesPerView="slidesPerView"
      :pagination="pagination"
      :breakpoints="breakpoints"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide class="slide-image" style="">
        <img src="../../../assets/Picture(3).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="">
        <img src="../../../assets/Picture(4).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="">
        <img src="../../../assets/Picture(3).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="">
        <img src="../../../assets/Picture(4).png" alt="" />
      </swiper-slide>

      <swiper-slide class="slide-image" style="">
        <img src="../../../assets/Picture(3).png" alt="" />
      </swiper-slide>

      <div style="display: flex; gap: 350px; margin-top: 50px">
        <div class="content">
          <h2 style="color: #534b42">Inspirations</h2>
          <p
            style="
              width: 359px;
              color: #706458;
              font-size: 18px;
              margin-bottom: 50px;
            "
          >
            Our experts are keen to stay on top of trends in order to offer you
            new inspirations for your interior and exterior every day. Remember
            that to inspire you we have to inspire ourselves and we want to
            share that with you.
          </p>
        </div>

        <div class="swiper-navigation" style="">
          <div style="display: flex; flex-direction: row; gap: 11px">
            <span class="custom-prev"
              ><img src="../../../assets/Button.svg" alt="" />
            </span>
            <span class="custom-next"
              ><img src="../../../assets/Button(1).svg" alt="" />
            </span>
          </div>

          <div class="swiper-pagination"></div>
        </div>
      </div>
    </swiper>
  </div>
</template>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Pagination, Navigation } from 'swiper/modules'
import 'swiper/css'
import 'swiper/css/navigation'

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const customPaginationRender = (swiper, current, total) => {
      return `${current.toString().padStart(2, '0')}/${total
        .toString()
        .padStart(2, '0')}`
    }
    return {
      slidesPerView: 1.5,
      modules: [Pagination, Navigation],
      breakpoints: {
        1024: {
          slidesPerView: 3.5,
          spaceBetween: 30,
        },
      },
      pagination: {
        el: '.swiper-pagination',
        clickable: true,
        type: 'custom',
        renderCustom: customPaginationRender,
      },
    }
  },
}
</script>

<style scoped>
.content {
  display: flex;
  gap: 140px;
  /* padding-top: 40px; */
}

.swiper-pagination {
  margin-bottom: 40px;
  font-size: 18px;
  font-weight: 400;
  color: #706458e5;
}

.custom-next {
  cursor: pointer;
}

.custom-prev {
  cursor: pointer;
}
* .swiper-navigation {
  margin-top: 48px;
  color: #a06056;
  font-size: 20px;
  font-weight: 700;
}

.mySwiper {
  padding-left: 150px;
}

.slide-image {
  object-fit: contain;
  width: 450px;
  height: 550px;
}
@media screen and (max-width: 768px) {
}
@media screen and (max-width: 1024px) {
  .mySwiper {
    padding-left: 70px;
  }
  .content {
    display: flex;
    gap: 100px;
    margin-top: 40px;
  }
}
</style>
