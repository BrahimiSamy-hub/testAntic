<template>
  <section>
    <div class="section">
      <div class="container">
        <h2 class="section-title">
          We stay by your side to design your projects
        </h2>

        <a href="#"
          ><span class="section-desc"
            >Find out more <img src="../../assets/Right.svg" alt="" /> </span
        ></a>
      </div>
      <aside class="services">
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

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Varta:wght@300..700&display=swap');

section {
  margin-bottom: 50px;
  margin-top: 64px;
}

.section-title {
  color: #534b42;
}

.section-desc {
  color: #a06056;
  font-size: 17px;
  font-weight: 700;
}

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

.container {
  display: grid;
  grid-template: repeat(1, 1fr);
  gap: 30px;
  max-width: 500px;
}

.services {
  display: grid;
  grid-template: repeat(1, 1fr) / repeat(2, 1fr);
  gap: 30px;
  /* max-width: 500px; */
}

.section {
  grid-template: repeat(1, 1fr) / repeat(2, 1fr);
  display: grid;
  margin-top: 64px;
  align-items: center;
}

@media screen and (max-width: 1024px) {
  /* section {
    margin-right: 50px;
    margin-left: 50px;
  } */

  .container {
    /* text-align: center; */
  }

  .section {
    grid-template-columns: 1fr;
    gap: 30px;
  }
}
@media screen and (max-width: 768px) {
  section {
    margin-right: 38px;
    margin-left: 38px;
  }

  /* .section,
  .container, */
  .services {
    grid-template-columns: 1fr;
    gap: 30px;
  }

  .services {
    /* grid-template-rows: repeat(4, auto); */
  }
}
</style>
