<template>
  <nav class="nav-menu nav-content" data-aos="fade-up" data-aos-duration="1500">
    <!-- Toggle Button for Mobile Menu -->
    <!-- <div class="menu-toggle">
      <button id="toggle-menu">
        <img src="../assets/Menu.svg" alt="" />
      </button>
    </div> -->
    <ul class="nav-items">
      <a href="#"
        ><li>
          <!-- <img src="../assets/Logotype.svg" alt="Logo" style="color: white" /> -->
          <Logo class="logo-desktop" />
          <LogoWhite class="logo-mobile" /></li
      ></a>
      <a href="#"><li class="nav-items">Products</li></a>
      <a href="#"><li class="nav-items">Rooms</li></a>
      <a href="#"><li class="nav-items">Services</li></a>
      <a href="#"><li class="nav-items">Inspirations</li></a>
      <a href="#"
        ><li class="nav-contact">
          <img src="../assets/Contact.svg" alt="Contact" /></li
      ></a>
    </ul>
  </nav>
</template>
<script>
import Logo from '@/components/Logo'
import LogoWhite from '@/components/LogoWhite.vue'
export default { components: { LogoWhite, Logo } }
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Varta:wght@300..700&display=swap');
i {
  font-family: 'Merriweather', serif;
}
.nav-menu {
  z-index: 1000;
  margin-left: 150px;
  position: absolute;
}
.nav-content {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  align-items: center;
}
a {
  text-decoration: none;
  color: #706458;
}
.nav-items {
  font-weight: 400;
  font-size: 18px;
  display: flex;
  align-items: center;
  gap: 45px;

  margin: 0;
  padding: 0;
}
.menu-toggle {
  display: none;
  padding: 10px;
}
.nav-contact {
  margin-left: 1000px;
}

.logo-desktop {
  display: block;
}

.logo-mobile {
  display: none;
}

@media screen and (max-width: 768px) {
  .nav-menu {
    /* padding-top: 10px; */
    position: absolute;
    width: 100%;
  }

  .nav-content {
    flex-direction: column;
    z-index: 100;
    transition: all 0.2s ease-out;
  }
  .nav-items {
    flex-direction: column;
  }
  i {
    display: block;
    text-align: right;
    padding: 0 10px 10px 0;
  }
  .menu-toggle {
    display: block;
    position: absolute;
    right: 10px;
    top: 10px;
  }

  .nav-items {
    display: none;
    flex-direction: column;
    width: 100%;
    align-items: center;
  }
}

@media screen and (max-width: 1386px) {
  .nav-items {
    color: #f7f8f9;
  }
  .nav-menu {
    margin-left: 70px;
  }
  .nav-contact {
    margin-left: 35px;
  }
  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }
}
</style>
