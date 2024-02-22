<template>
  <div class="menu" data-aos="fade-up" data-aos-duration="1500">
    <nav>
      <ul>
        <a href="#"
          ><div>
            <Logo class="logo-desktop" />
            <LogoWhite class="logo-mobile" /></div
        ></a>
        <li><a href="#">roducts</a></li>
        <li><a href="#">Rooms</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Inspirations</a></li>
      </ul>
    </nav>
    <a href="#"
      ><li class="img">
        <img src="../assets/Contact.svg" alt="Contact" /></li
    ></a>
  </div>
</template>

<script>
import Logo from '@/components/Logo'
import LogoWhite from '@/components/LogoWhite.vue'

export default { components: { LogoWhite, Logo } }
</script>

<style scoped>
/* @import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Varta:wght@300..700&display=swap'); */

.menu {
  z-index: 1000;
  position: absolute;
  margin-top: 70px;
  margin-left: 150px;
  margin-right: 150px;
  display: flex;
  align-items: center;
}

a {
  text-decoration: none;
  color: #706458;
  font-weight: 400;
  font-size: 18px;
}

nav li {
  padding-top: 7px;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 24px;
  align-items: center;
  justify-content: center;
}

i {
  font-family: 'Merriweather', serif;
}

.logo-desktop {
  display: block;
}

.logo-mobile {
  display: none;
}
.img {
  margin-left: 1100px;
}

@media screen and (max-width: 768px) {
  li a {
    display: none;
  }
  .menu {
    margin-top: 50px;
    margin-left: 32px;
  }

  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }
}

@media only screen and (max-width: 1300px) and (min-width: 768px) {
  a {
    color: #f7f8f9;
  }

  .menu {
    margin-left: 70px;
  }

  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }

  nav ul {
    list-style: none;
    display: flex;
    gap: 50px;
    align-items: center;
    justify-content: center;
  }

  .img {
    margin-left: 50px;
  }
}
</style>
