<template>
  <div class="navbar">
    <h3>Sobre mí</h3>
    <h3>Skills</h3>
    <h3>Portafolio</h3>
    <button>CONTACTO</button>
  </div>
  <div class="navbar_m">
    <img src="../assets/menu.svg" alt="menu" @click="menu" />
  </div>
  <div :class="'menu ' + clase">
    <h3>Sobre mí</h3>
    <h3>Skills</h3>
    <h3>Portafolio</h3>
    <button>CONTACTO</button>
  </div>
</template>
<script>
export default {
  methods: {
    menu() {
      this.clase = this.clase == "close" ? "open" : "close";
    },
  },
  data() {
    return {
      openmenu: false,
      clase: "close",
    };
  },
};
</script>

<style scoped>
.navbar {
  background-color: #000;
  width: 100%;
  height: 4.5rem;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
.navbar_m,
.menu {
  display: none;
}

h3 {
  color: #fff;
  margin: 0 2rem;
  cursor: pointer;
}

button {
  height: 2.8rem;
  width: 8rem;
  border-radius: 30px;
  font-size: 15px;
  font-weight: bold;
  margin-right: 1rem;
  cursor: pointer;
}

@media screen and (max-width: 768px) {
  .navbar {
    display: none;
  }
  .navbar_m {
    height: 4.5rem;
    display: flex;
    background: #000;
    justify-content: flex-end;
  }

  .navbar_m img {
    margin: 1rem;
    width: 2.5rem;
  }

  .menu {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #000;
    width: 100%;
  }

  .open {
    height: 15rem;
    transition: height 1s;
  }

  .close {
    height: 0;
    transition: height 1s;
  }

  .close h3 {
    opacity: 0;
    transition: opacity 0.5s;
    z-index: -1;
  }
  .close button {
    opacity: 0;
    transition: opacity 0.5s;
    z-index: -1;
  }

  .open h3 {
    opacity: 1;
    transition: opacity 0.1s;
  }

  .open button {
    opacity: 1;
    transition: opacity 0.1s;
  }

  .menu h3 {
    margin: 1rem 0;
    font-weight: normal;
  }

  .menu button {
    width: 100%;
    margin: 0;
    border-radius: 0;
    outline: none;
    border: none;
    text-decoration: none;
  }
}
</style>
