<template>
  <div
    data-aos="fade-up"
    data-aos-duration="1500"
    style="background-color: white"
  >
    <article style="">
      <h2 class="grid-title">Inspirations</h2>
      <p style="max-width: 400px" class="grid-p">
        Our experts are keen to stay on top of trends in order to offer you new
        inspirations for your interior and exterior every day. Remember that to
        inspire you we have to inspire ourselves and we want to share that with
        you.
      </p>
    </article>
    <div class="grid-container">
      <figure>
        <img src="../../../assets/Picture(3).png" alt="Image 1" />
        <figcaption>Chair</figcaption>
      </figure>
      <figure>
        <img src="../../../assets/Picture(4).png" alt="Image 2" />
        <figcaption>Cooked</figcaption>
      </figure>
      <figure>
        <img src="../../../assets/1.jpeg" alt="Image 3" />
        <figcaption>Living room</figcaption>
      </figure>
      <figure>
        <img src="../../../assets/2.jpeg" alt="Image 4" />
        <figcaption>Tables</figcaption>
      </figure>
    </div>
  </div>
</template>
<script></script>

<style scoped>
.grid-container {
  margin-top: 50px;
  padding-bottom: 50px;
  display: grid;
  grid-template-columns: calc(50% - 5px) calc(50% - 5px);
  gap: 10px;
}

img {
  height: 175px;
  object-fit: cover;
}
figure {
  margin: 0;
  object-fit: contain;
}
figcaption {
  font-family: lato, sans-serif;
  padding-top: 10px;
  color: #121212;
  font-weight: 400;
  font-size: 15px;
}
img {
  width: 100%;
}
.grid-p {
  font-size: 18px;
  color: #706458e5;
  font-weight: 400;
}
.grid-title {
  margin-top: 64px;
  margin-bottom: 20px;
  font-size: 35px;
  color: #534b42;
  font-weight: 400;
}
</style>
