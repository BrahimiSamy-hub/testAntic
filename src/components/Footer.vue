<template>
  <footer class="footer">
    <div class="links">
      <span><img src="../assets/LogotypeFooter.svg" alt="" /></span>
      <ul>
        <li class="title">Products</li>
        <ul class="sub-title">
          <a href=""><li>Furniture</li></a>
          <a href=""><li>Decoration</li></a>
          <a href=""><li>Storage</li></a>
          <a href=""><li>Storage</li></a>
          <a href=""><li>Connected home</li></a>
        </ul>
      </ul>
      <ul>
        <li class="title">Rooms</li>
        <ul class="sub-title">
          <a href=""><li>Living room</li></a>
          <a href=""><li>Dining room</li></a>
          <a href=""><li>Cooked</li></a>
          <a href=""><li>Bedroom</li></a>
          <a href=""><li>Bathroom</li></a>
          <a href=""><li>Office</li></a>
          <a href=""><li>Laundry</li></a>
          <a href=""><li>Garage</li></a>
        </ul>
      </ul>
      <ul>
        <li class="title">Services</li>
        <ul class="sub-title">
          <a href=""><li>Click and collect</li></a>
          <a href=""><li>Conception</li></a>
          <a href=""><li>Installation</li></a>
          <a href=""><li>Advices</li></a>
          <a href=""><li>Gift card</li></a>
        </ul>
      </ul>
      <ul>
        <li class="title">About</li>
        <ul class="sub-title">
          <a href=""><li>Our story</li></a>
          <a href=""><li>Our stores</li></a>
          <a href=""><li>Our partners</li></a>
        </ul>
      </ul>
      <ul>
        <li class="title">We respect our planet</li>
        <ul class="">
          <img src="../assets/Picture(6).png" alt="" />
          <p class="item-p">
            We’re taking positive steps to reduce <br />
            our impact on the planet <br />
            For us, that means retailing <br />
            responsibly.
          </p>
          <a href="#" class="item-a"
            >Learn more <img src="../assets/Right.svg" alt=""
          /></a>
        </ul>
      </ul>
    </div>
    <div>
      <ul class="social">
        <li>
          <a href=""><img src="../assets/Facebook.svg" alt="" /></a>
        </li>
        <li>
          <a href=""><img src="../assets/Twitter.svg" alt="" /></a>
        </li>
        <li>
          <a href=""><img src="../assets/Linkedin.svg" alt="" /></a>
        </li>
        <li>
          <a href=""><img src="../assets/Instagram.svg" alt="" /></a>
        </li>
      </ul>
      <ul
        style="
          /* display: flex; */
          /* justify-content: space-between; */
          /* flex-direction: row; */
        "
      >
        <ul
          style="
            display: flex;
            margin-top: 20px;
            margin-bottom: 20px;
            gap: 20px;
            /* justify-content: space-between;   */
            /* justify-content: center; */
            flex-direction: end;
          "
        >
          <li>
            <a href=""><span>Privacy policy</span></a>
          </li>
          <li>
            <a href=""><span>Term of service</span></a>
          </li>

          <li>
            <a href=""><span>Language</span></a>
          </li>
        </ul>
        <p class="copyright" style="justify-content: center">
          &copy; {{ new Date().getFullYear() }} Agence Dnd
        </p>
      </ul>
    </div>
  </footer>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Varta:wght@300..700&display=swap');
snap {
  font-family: 'Varta', sans-serif;
}
.social {
  display: flex;
  gap: 20px;
  justify-content: center;
  margin-top: 48px;
}

.footer {
  margin-top: 70px;
  margin-right: 150px;
  margin-left: 150px;
}

.item-p {
  color: #706458;
  font-size: 16px;
  font-weight: 400;
  margin-bottom: 15px;
}

.item-a {
  color: #a06056;
  font-size: 17px;
  font-weight: 700;
}

.title {
  margin-bottom: 22px;
  color: #534b42;
  font-weight: 600;
  font-size: 25px;
}

.sub-title {
  display: flex;
  flex-direction: column;
  gap: 12px;
  color: #706458;
  font-weight: 400;
  font-size: 18px;
}

.copyright {
  color: #706458;
  font-weight: 400;
  font-size: 18px;
  margin-bottom: 48px;
  text-align: center;
}

.links {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
@media (max-width: 1024px) {
  .title {
    margin-bottom: 22px;
    color: #534b42;
    font-weight: 600;
    font-size: 25px;
  }

  .sub-title {
    display: flex;
    flex-direction: column;
    gap: 12px;
    color: #706458;
    font-weight: 400;
    font-size: 18px;
  }
  .footer {
    margin-top: 48px;
    margin-right: 50px;
    margin-left: 50px;
  }
}
@media screen and (max-width: 768px) {
  .links {
    gap: 48px;
    flex-direction: column;
    /* justify-content: space-between; */
  }
  .title {
    margin-bottom: 22px;
    color: #534b42;
    font-weight: 600;
    font-size: 25px;
  }

  .sub-title {
    display: flex;
    flex-direction: column;
    gap: 12px;
    color: #706458;
    font-weight: 400;
    font-size: 18px;
  }
  .footer {
    margin-top: 48px;
    margin-right: 32px;
    margin-left: 32px;
  }
}
</style>
