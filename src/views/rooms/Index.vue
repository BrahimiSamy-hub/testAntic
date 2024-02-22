<template>
  <section>
    <h1 class="main-title">Find you room</h1>
    <div class="container">
      <p class="main-p">
        Dining room, bedroom, bathroom or office. Find what you need
      </p>

      <swiper
        :navigation="{
          nextEl: '.custom-next',
          prevEl: '.custom-prev',
        }"
        :pagination="{
          clickable: true,
          el: '.swiper-pagination',
        }"
        :loop="true"
        :breakpoints="breakpoints"
        :modules="modules"
        class="mySwiper"
      >
        <swiper-slide>
          <h2 class="slide-title">Bedroom</h2>

          <img
            src="../../assets/Picture_1_.webp"
            loading="lazy"
            alt=""
            class="slide-image"
          />
          <p class="slide-p">New arrivals</p>
        </swiper-slide>

        <swiper-slide>
          <h2 class="slide-title">Living room</h2>
          <img
            src="../../assets/Picture_2_.webp"
            loading="lazy"
            alt=""
            class="slide-image"
          />
          <p class="slide-p">New arrivals</p>
        </swiper-slide>

        <swiper-slide>
          <h2 class="slide-title">Bedroom</h2>
          <img
            src="../../assets/Picture_1_.webp"
            loading="lazy"
            alt=""
            class="slide-image"
          />
          <p class="slide-p">New arrivals</p>
        </swiper-slide>

        <swiper-slide>
          <h2 class="slide-title">Living room</h2>
          <img
            src="../../assets/Picture_2_.webp"
            loading="lazy"
            alt=""
            class="slide-image"
          />
          <p class="slide-p">New arrivals</p>
        </swiper-slide>

        <div class="swiper-navigation">
          <span class="custom-next"
            >Next
            <img src="../../assets/Right.svg" alt="" />
          </span>
          <!-- <div class="swiper-pagination"></div> -->
        </div>
      </swiper>
    </div>
  </section>
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
          slidesPerView: 2,
          spaceBetween: 10,
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

.container {
  display: flex;
  gap: 24px;
}

.swiper-navigation {
  margin-top: 48px;
  color: #a06056;
  font-size: 20px;
  font-weight: 700;
}
.swiper {
  margin-bottom: 50px;
  width: 100%;
  height: 100%;
}
.swiper-slide {
  display: flex;
  align-items: center;
}
.slide-title {
  position: absolute;
  color: #a06056;
  margin-left: 100px;
}
.slide-p {
  color: #706458e5;
  font-size: 18px;
  font-weight: 400;
  align-self: flex-start;
  margin-left: 32px;
}
.slide-image {
  object-fit: contain;
}
.main-title {
  font-weight: 400;
  color: #706458;
  margin-top: 64px;
  font-size: 55px;
  margin-bottom: 48px;
}
.main-p {
  width: 165px;
  font-size: 18px;
  font-weight: 400;
  color: #706458e5;
}
@media screen and (max-width: 768px) {
  section {
    margin-left: 38px;
    margin-right: 38px;
  }

  .swiper-navigation {
    margin-top: 33px;
  }

  .main-p {
    width: 310px;
    margin-bottom: 33px;
  }

  .main-title {
    margin-top: 48px;
    font-size: 35px;
    margin-bottom: 20px;
  }

  .container {
    display: block;
    gap: 16px;
  }

  .slide-image {
    height: 230px;
  }
}

@media screen and (max-width: 1024px) {
  .swiper-navigation {
    margin-top: 33px;
  }

  .main-p {
    width: 310px;
    margin-bottom: 33px;
  }

  .main-title {
    margin-top: 48px;
    font-size: 35px;
    margin-bottom: 20px;
  }

  .container {
    display: block;
    gap: 16px;
  }
  .slide-image {
    height: 230px;
  }
}
</style>
