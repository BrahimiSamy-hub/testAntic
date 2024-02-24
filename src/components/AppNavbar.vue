<!-- <template>
  <div class="menu" data-aos="zoom-in" data-aos-duration="1500">
    <nav>
      <ul>
        <a href="#"
          ><div>
            <Logo class="logo-desktop" />
            <LogoWhite class="logo-mobile" /></div
        ></a>
        <li><a href="#">Products</a></li>
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
  padding-top: 8px;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 32px;
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
</style> -->
<template>
  <header>
    <div class="navbar" style="position: absolute; z-index: 9999">
      <div>
        <ul class="links">
          <li>
            <a href="#">
              <Logo class="logo-desktop" /> <LogoWhite class="logo-mobile"
            /></a>
          </li>
          <li class="show"><a href="#">Products</a></li>
          <li class="show"><a href="#">Rooms</a></li>
          <li class="show"><a href="#">Services</a></li>
          <li class="show"><a href="#">Inspirations</a></li>
        </ul>
      </div>

      <a href="#" class="action-btn" style="color: white"
        ><img src="../assets/Contact.svg" alt=""
      /></a>
      <div class="toggle-btn">
        <button style="background-color: transparent; border: none">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            x="0px"
            y="0px"
            width="40"
            height="40"
            viewBox="0,0,256,256"
          >
            <g
              fill="#ffffff"
              fill-rule="nonzero"
              stroke="none"
              stroke-width="1"
              stroke-linecap="butt"
              stroke-linejoin="miter"
              stroke-miterlimit="10"
              stroke-dasharray=""
              stroke-dashoffset="0"
              font-family="none"
              font-weight="none"
              font-size="none"
              text-anchor="none"
              style="mix-blend-mode: normal"
            >
              <g transform="scale(8.53333,8.53333)">
                <path
                  d="M3,7c-0.36064,-0.0051 -0.69608,0.18438 -0.87789,0.49587c-0.18181,0.3115 -0.18181,0.69676 0,1.00825c0.18181,0.3115 0.51725,0.50097 0.87789,0.49587h24c0.36064,0.0051 0.69608,-0.18438 0.87789,-0.49587c0.18181,-0.3115 0.18181,-0.69676 0,-1.00825c-0.18181,-0.3115 -0.51725,-0.50097 -0.87789,-0.49587zM3,14c-0.36064,-0.0051 -0.69608,0.18438 -0.87789,0.49587c-0.18181,0.3115 -0.18181,0.69676 0,1.00825c0.18181,0.3115 0.51725,0.50097 0.87789,0.49587h24c0.36064,0.0051 0.69608,-0.18438 0.87789,-0.49587c0.18181,-0.3115 0.18181,-0.69676 0,-1.00825c-0.18181,-0.3115 -0.51725,-0.50097 -0.87789,-0.49587zM3,21c-0.36064,-0.0051 -0.69608,0.18438 -0.87789,0.49587c-0.18181,0.3115 -0.18181,0.69676 0,1.00825c0.18181,0.3115 0.51725,0.50097 0.87789,0.49587h24c0.36064,0.0051 0.69608,-0.18438 0.87789,-0.49587c0.18181,-0.3115 0.18181,-0.69676 0,-1.00825c-0.18181,-0.3115 -0.51725,-0.50097 -0.87789,-0.49587z"
                ></path>
              </g>
            </g>
          </svg>
        </button>
      </div>
    </div>
    <div class="dropdown-menu">
      <li><a style="color: white" href="#">Products</a></li>
      <li><a style="color: white" href="#">Rooms</a></li>
      <li><a style="color: white" href="#">Services</a></li>
      <li><a style="color: white" href="#">Inspirations</a></li>
    </div>
  </header>
</template>

<script>
import Logo from '@/components/Logo'
import LogoWhite from '@/components/LogoWhite.vue'

export default { components: { LogoWhite, Logo } }

document.addEventListener('DOMContentLoaded', function () {
  const toggleBtn = document.querySelector('.toggle-btn button')
  const dropDownMenu = document.querySelector('.dropdown-menu')

  function toggleDropdown() {
    dropDownMenu.classList.toggle('open')
  }

  toggleBtn.addEventListener('click', function () {
    toggleDropdown()
  })

  document.addEventListener('click', function (e) {
    if (!dropDownMenu.contains(e.target) && !toggleBtn.contains(e.target)) {
      if (dropDownMenu.classList.contains('open')) {
        dropDownMenu.classList.remove('open')
      }
    }
  })
})
</script>

<style scoped>
a {
  color: #706458;
}
.navbar {
  padding: 55px 150px;
  width: calc(100% - 300px);
  height: 60px;
  max-width: 1600px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo-desktop {
  display: block;
}

.logo-mobile {
  display: none;
}

.dropdown-menu {
  display: none;
  z-index: 9999999;
  position: absolute;
  right: 2rem;
  top: 100px;
  height: 0;
  width: 200px;
  margin-right: 72px;
  background: rgba(225, 255, 255, 0.1);
  backdrop-filter: blur(15px);
  overflow: hidden;
  border-radius: 10px;
  transition: height 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275);
}

.dropdown-menu li {
  font-size: 25px;
  line-height: 1.2;
  padding: 0.7rem;
  display: flex;
  align-items: center;
  justify-content: center;
}

.dropdown-menu.open {
  height: 205px;
}

.links {
  font-size: 18px;
  font-weight: 400px;
  align-items: center;
  display: flex;
  gap: 32px;
}

.navbar .toggle-btn {
  cursor: pointer;
  display: none;
}

@media (max-width: 1375px) {
  .dropdown-menu {
    display: block;
  }
  .navbar {
    width: calc(100% - 200px);
    padding: 55px 100px;
  }
  .show,
  .action-btn {
    display: none;
  }
  .navbar .toggle-btn {
    display: block;
  }
  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }
}

@media (max-width: 768px) {
  .navbar {
    width: calc(100% - 64px);
    padding: 45px 32px;
  }

  .dropdown-menu {
    left: 2rem;
    margin-right: 0;
    width: unset;
  }
  .logo-desktop {
    display: none;
  }

  .logo-mobile {
    display: block;
  }
}
</style>
