<template>
  <div
    style="margin-left: 32px; margin-right: 32px"
    data-aos="fade-up"
    data-aos-duration="1500"
  >
    <h2 class="grid-title">Inspirations</h2>
    <p style="min-width: 310px" class="grid-p">
      Our experts are keen to stay on top of trends in order to offer you new
      inspirations for your interior and exterior every day. Remember that to
      inspire you we have to inspire ourselves and we want to share that with
      you.
    </p>
    <div class="container">
      <div class="container-img" data-aos="fade-up" data-aos-duration="1500">
        <img
          src="../../../assets/Picture(3).png"
          alt=""
          style="object-fit: contain"
        />
        <span style="margin-top: 15px"> Chair</span>
      </div>

      <div class="container-img" data-aos="fade-up" data-aos-duration="1500">
        <img
          src="../../../assets/Picture(4).png"
          alt=""
          style="object-fit: contain"
        />
        <span style="margin-top: 15px"> Cooked</span>
      </div>
      <div class="container-img">
        <img
          src="../../../assets/Picture(6).png"
          alt=""
          style="object-fit: fill; height: 175px"
        />
        <span style="margin-top: 15px"> Living room</span>
      </div>
      <div class="container-img">
        <img
          src="../../../assets/Picture(5).png"
          alt=""
          style="object-fit: fill; height: 175px"
        />
        <span style="margin-top: 15px"> Tables</span>
      </div>
    </div>
  </div>
</template>
<script></script>

<style scoped>
.grid-p {
  font-size: 18px;
  color: #706458e5;
  font-weight: 400;
  margin-bottom: 40px;
}
.grid-title {
  margin-top: 64px;
  margin-bottom: 20px;
  font-size: 35px;
  color: #534b42;
  font-weight: 400;
}

.container-img {
  display: flex;
  flex-direction: column;
  width: 145px;
}

.container {
  display: grid;
  grid-template-columns: 145px 145px;
  grid-row: auto auto;
  grid-column-gap: 20px;
  grid-row-gap: 20px;
  padding-bottom: 48px;
}
</style>
