<template>
  <header>
    <a href="#" class="logo">
      <i class="ri-cloud-fill"></i>
      <span>logo</span></a
    >
    <ul class="navbar">
      <li><a href="#" class="active">Home</a></li>
      <li><a href="#">About Us</a></li>
      <li><a href="#">Category</a></li>
      <li><a href="#">Contact</a></li>
    </ul>

    <div class="main">
      <a href="#" class="user"> Sign in </a>
      <a href="#">Register</a>

      <div class="bx bx-menu" id="menu-icon">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
        >
          <path
            fill-rule="evenodd"
            d="M2 4.75A.75.75 0 012.75 4h14.5a.75.75 0 010 1.5H2.75A.75.75 0 012 4.75zM2 10a.75.75 0 01.75-.75h14.5a.75.75 0 010 1.5H2.75A.75.75 0 012 10zm0 5.25a.75.75 0 01.75-.75h14.5a.75.75 0 010 1.5H2.75a.75.75 0 01-.75-.75z"
            clip-rule="evenodd"
          />
        </svg>
      </div>
    </div>
  </header>
</template>

<script>
import SvgIcon from "@jamescoyle/vue-icon";
import { mdiAbTesting } from "@mdi/js";

export default {
  components: {
    SvgIcon,
  },

  data() {
    return {
      path: mdiAbTesting,
    };
  },

  mounted(){
    let menu = document.querySelector('#menu-btn');
    let navbar = document.querySelector('.navbar');

    menu.onclick = () => {
      menu.classList.toggle('bx-x');
      navbar.classList.toggle('open');
    }
  }

};
</script>

<style scoped>
header {
  position: fixed;
  width: 100%;
  top: 0;
  right: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: transparent;
  padding: 28px 12px;
  transition: all 0.5s ease;
}

.logo {
  display: flex;
  align-items: center;
}

.logo i {
  color: #000;
  font-size: 28px;
  margin-right: 3px;
}

.logo span {
  color: green;
  font-size: 1.1rem;
  font-weight: 600;
}

.navbar {
  display: flex;
}

.navbar a {
  color: #000;
  font-size: 1.1rem;
  font-weight: 600;
  padding: 7px 0;
  margin: 0px 7px;
  transition: all 0.5s ease;
}

.navbar a:hover {
  color: green;
}

.navbar a.active {
  color: green;
}

.main {
  display: flex;
  align-items: center;
}

.main a {
  margin-right: 25px;
  margin-left: 10px;
  color: #000;
  font-size: 1.1rem;
  font-weight: 600;
  transition: all 0.5s ease;
}

.user {
  display: flex;
  align-items: center;
}

.main a:hover {
  color: green;
}

#menu-icon {
  font-size: 35px;
  color: #000;
  cursor: pointer;
  z-index: 10001;
  display: none;
}

@media (max-width: 1280px) {
  header {
    padding: 14px 2%;
    transition: 0.2s;
  }
  .navbar a {
    padding: 5px 0;
    margin: 0px 20px;
  }
}

@media (max-width: 1090px) {
  #menu-icon {
    display: block;
  }
  .navbar {
    position: absolute;
    top: 100%;
    right: -100%;
    width: 270px;
    height: 29vh;
    background: green;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    border-radius: 10px;
    transition: all 0.5s ease;
  }
  .navbar a {
    display: block;
    margin: 12px 0;
    padding: 0px 25px;
    transition: all 0.5s ease;
  }

  .navbar a:hover {
    color: aliceblue;
    transform: translateY(5px);
  }

  .navbar a.active {
    color: white;
  }

  .navbar.open {
    right: 2%;
  }
}
</style>
