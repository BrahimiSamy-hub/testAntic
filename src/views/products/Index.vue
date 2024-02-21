<template>
  <section style="min-height: 500px">
    <div class="container2">
      <div class="text-content3">
        <h2 style="color: #534b42">
          We stay by your side to design your projects
        </h2>
        <a href="#"
          ><span style="color: #a06056; font-size: 17px; font-weight: 700"
            >Find out more <img src="../../assets/Right.svg" alt="" /> </span
        ></a>
      </div>
      <aside class="text-content4">
        <div>
          <span class="services-title">Our Advices</span>
          <p class="services-desc">
            What if you took advantage of this rather special period to rethink
            your interior? You spend more time at home so you might as well feel
            good there.
          </p>
        </div>
        <div>
          <span class="services-title">Click and Collect</span>
          <p class="services-desc">
            Adapted and contactless. Free from € 200 of purchases in stores
            offering the service.
          </p>
        </div>
        <div>
          <span class="services-title">Conception Service</span>
          <p class="services-desc">
            Personalized service with an expert advisor for your interior and
            exterior decoration or layout projects.
          </p>
        </div>
        <div>
          <span class="services-title">Installation Service</span>
          <p class="services-desc">
            Our furniture packaged in flat packs are designed for easy assembly.
            But you can call on our partner.
          </p>
        </div>
      </aside>
    </div>
  </section>
</template>
<script></script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Varta:wght@300..700&display=swap');
.services-title {
  font-size: 25px;
  font-weight: 400;
  color: #a06056;
}
.services-desc {
  font-size: 18px;
  font-weight: 400;
  color: #706458e5;
}
.text-content3 {
  display: grid;
  grid-template: repeat(1, 1fr);
  gap: 30px;
  max-width: 500px;
}
.text-content4 {
  display: grid;
  grid-template: repeat(1, 1fr) / repeat(2, 1fr);
  gap: 30px;
  /* max-width: 500px; */
}
.container2 {
  grid-template: repeat(1, 1fr) / repeat(2, 1fr);
  display: grid;
  margin-right: 150px;
  margin-left: 150px;
  margin-top: 64px;
  align-items: center;
}

@media screen and (max-width: 768px) {
  .container2 {
    margin-right: 32px;
    margin-left: 32px;
  }
  .container2,
  .text-content3,
  .text-content4 {
    grid-template-columns: 1fr;
    gap: 30px;
  }

  .text-content4 {
    grid-template-rows: repeat(4, auto);
  }
}
@media screen and (max-width: 1024px) {
  .container2 {
    margin-right: 50px;
    margin-left: 50px;
    grid-template-columns: 1fr;
    gap: 30px;
  }
}
</style>
