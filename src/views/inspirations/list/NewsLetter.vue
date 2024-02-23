<template>
  <div class="content">
    <div class="text">
      <h2 class="content-title">Be aware of the latest trends</h2>
      <p class="content-paragraphe">
        Stay informed of new trends, but also of our various offers.
      </p>
      <a href="#"
        ><span>Learn more </span><img src="../../../assets//Right.svg" alt=""
      /></a>
    </div>
    <aside class="input subscription-form">
      <input
        type="email"
        id="newsletter-email"
        placeholder="email@address.com"
        required
      />
      <button type="submit" id="subscribe-button">Subscribe</button>
    </aside>
  </div>
</template>

<script></script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Varta:wght@300..700&display=swap');

.content-title {
  font-size: 35px;
  color: #121212;
}
.content-paragraphe {
  font-size: 18px;
  color: #706458e5;
}
span {
  font-size: 17px;
  color: #a06056;
}

.content {
  margin-right: 150px;
  margin-left: 150px;
  display: flex;

  gap: 159;
  justify-content: space-between;
  align-items: center;
  /* margin-top: 70px; */
}

.text {
  margin-bottom: 64px;
  margin-top: 70px;
  gap: 16px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
}

.input {
  display: flex;
  gap: 10px;
  height: 50px;
}

h2 {
  font-size: 35px;
}

input {
  text-decoration: none;
  width: 296px;
  background-color: #f3eee84d;
  border: none;
}

.subscription-form input[type='email'] {
  padding: 10px;
  font-size: 18px;
}

.subscription-form button {
  padding: 10px 20px;
  background-color: #534b42;
  color: white;
  border: none;
  cursor: pointer;
  font-size: 17px;
}

@media screen and (max-width: 768px) {
  .text {
    margin-top: 50px;
    margin-bottom: 32px;
  }
  .content {
    margin-left: 32px;
    margin-right: 32px;
    flex-direction: column;
    align-items: start;
  }
  .subscription-form {
    display: flex;
    flex-direction: column;
  }
}

@media screen and (min-width: 768px) and (max-width: 1024px) {
  .content {
    display: block;
    margin-right: 70px;
    margin-left: 70px;
  }

  .subscription-form {
    margin-bottom: 50px;
  }
}
</style>
