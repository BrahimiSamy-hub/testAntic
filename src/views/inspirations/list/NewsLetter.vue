<template>
  <section style="min-height: 800px; background-color: white">
    <div class="container">
      <div class="text-content">
        <h2 style="font-size: 35px; font-weight: 400">
          Be aware of the latest trends
        </h2>
        <div style="display: grid; gap: 10px">
          <p style="color: #706458e5; font-size: 18px; font-weight: 400">
            Stay informed of new trends, but also of our various offers.
          </p>
          <a href="#"
            ><span style="color: #a06056; font-size: 17px; font-weight: 700"
              >Learn more </span
            ><img src="../../../assets//Right.svg" alt=""
          /></a>
        </div>
      </div>
      <aside class="text-content2">
        <input
          style="width: 296px; background-color: #f3eee84d"
          type="email"
          id="newsletter-email"
          placeholder="email@address.com"
          required
        />
        <button
          style="background-color: #534b42; color: white; width: 143px"
          type="submit"
          id="subscribe-button"
        >
          Subscribe
        </button>
      </aside>
    </div>
  </section>
</template>
<script></script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Varta:wght@300..700&display=swap');
.text-content > h2 {
  color: #121212;
}
.text-content {
  display: grid;
  height: 200px;
  grid-template: repeat(1, 1fr);
  /* gap: 18px; */
  margin-top: 70px;
  /* max-width: 500px; */
}
.text-content2 {
  /* display: grid;

  
  grid-template: repeat(3, 1fr) / repeat(2, 1fr); */
  display: flex;
  gap: 10px;
  height: 50px;
  margin-right: 150px;
  margin-left: 150px;
}
.container {
  grid-template: repeat(1, 1fr) / repeat(2, 1fr);
  display: flex;
  margin-right: 150px;
  margin-left: 150px;
  justify-content: space-between;
  align-items: center;
}

@media screen and (max-width: 768px) {
  .container {
    margin-right: 32px;
    margin-left: 32px;
  }
  .container,
  .text-content,
  .text-content2 {
    grid-template-columns: 1fr;
    gap: 20px;
  }
  .text-content2 {
    grid-template-rows: repeat(4, auto);
  }
}
</style>
