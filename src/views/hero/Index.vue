<template>
  <section class="container-hero">
    <div class="text-content-hero">
      <small class="small-hero">Home Design</small>
      <h1 class="title-hero">Elegance for Interiors & Exteriors</h1>
      <p class="desc-hero">
        We provide everyone with modern, trendy, quality furniture
      </p>
      <a href="#">
        <img src="../../assets/Scroll Down.svg" alt="" />
      </a>
    </div>
    <div class="heroImg">
      <img src="../../assets/Picture.png" alt="My Image" />
    </div>
  </section>
</template>
<script></script>
<style>
.text-content-hero {
  margin-left: 150px;
  display: grid;
  max-width: 420px;
  position: absolute;
  gap: 30px;
  grid-template: 1fr;
}
.container-hero {
  display: flex; /* Use flexbox layout */
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
  width: 50%;
}
@media (max-width: 1120px) {
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
    margin-left: 50px;
    max-width: 400px;
  }
  .container-hero {
    justify-content: center;
  }
  .heroImg > img {
    height: 100vh;
    width: 100%;
  }
}
@media screen and (max-width: 768px) {
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
  }
}
</style>
