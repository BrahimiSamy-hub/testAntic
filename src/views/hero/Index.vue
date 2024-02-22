<template>
  <div class="container-hero" style="">
    <div class="text-content-hero">
      <small class="small-hero">Home Design</small>
      <h1 class="title-hero">Elegance for Interiors & Exteriors</h1>
      <p class="desc-hero">
        We provide everyone with modern, trendy, quality furniture
      </p>
      <a href="#" style="display: flex">
        <ScrollDown class="logo-desktop" />
        <ScrollDownWhite class="logo-mobile" />
      </a>
    </div>
    <div class="heroImg">
      <img src="../../assets/Picture.jpeg" loading="lazy" alt="My Image" />
    </div>
  </div>
</template>

<script>
import ScrollDown from '@/components/ScrollDown.vue'
import ScrollDownWhite from '@/components/ScrollDownWhite.vue'

export default { components: { ScrollDownWhite, ScrollDown } }
</script>

<style scoped>
.logo-desktop {
  display: block;
}

.logo-mobile {
  display: none;
}
.text-content-hero {
  display: grid;
  max-width: 420px;
  position: absolute;
  gap: 30px;
  grid-template: 1fr;
}
.container-hero {
  padding-left: 150px;
  display: flex;
  align-items: center;
}
.title-hero {
  color: #a06056;
  font-size: 50px;
  font-weight: 400;
}
.small-hero {
  color: #a06056;
  font-size: 14px;
  font-weight: 700;
}
.desc-hero {
  color: #706458e5;
  font-size: 22px;
  font-weight: 400;
}
.heroImg {
  text-align: end;
  width: 100%;
  /* position: absolute; */
}
.heroImg > img {
  height: 100vh;
  width: 60%;
  object-fit: cover;
}
@media (max-width: 1300px) {
  .title-hero {
    color: #ffffff;
    font-size: 35px;
  }
  .small-hero {
    color: #ffffff;
  }
  .desc-hero {
    color: #ffffff;
    font-size: 18px;
  }
  .text-content-hero {
    /* text-align: center;

    margin-left: 50px;
    max-width: 400px; */
    display: flex;
    text-align: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    max-width: 420px;
    width: 100%;
  }
  .container-hero {
    padding-left: 0px;
    justify-content: center;
  }
  .heroImg > img {
    height: 100vh;
    width: 100%;
    object-fit: cover;
  }
  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }
}

@media screen and (max-width: 768px) {
  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }

  .title-hero {
    color: #ffffff;
    font-size: 35px;
  }

  .small-hero {
    color: #ffffff;
  }

  .desc-hero {
    color: #f7f8f9;
    font-size: 18px;
  }

  .text-content-hero {
    text-align: center;
    margin-left: 25px;
    max-width: 325px;
  }

  .container-hero {
    justify-content: center;
  }

  .heroImg > img {
    height: 100vh;
    width: 100%;
    object-fit: cover;
  }
}
</style>
