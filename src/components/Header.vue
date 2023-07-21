<script setup>
import Logo from "../assets/img/logo_header.png";
import { ref } from "vue";

const navBarVisible = ref(false);

const toggleNavBar = () => {
  navBarVisible.value = !navBarVisible.value;
};
</script>

<template>
  <div class="header">
    <img :src="Logo" alt="logo" class="logo" width="150" />
    <div class="bars" @click="toggleNavBar">
      <div class="line"></div>
      <div class="line"></div>
      <div class="line"></div>
    </div>
    <nav class="nav_bar" :class="{ active: navBarVisible }">
      <ul>
        <li><a href="#" class="active">Inicio</a></li>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Inicio</a></li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
.header {
  width: 100%;
  height: 80px;
  background-color: var(--morado-oscuro);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 100px;
}
.logo img {
  max-height: 100%; /* Ajustamos la altura al 100% del contenedor */
  max-width: 100%; /* Ajustamos el ancho al 100% del contenedor */
}
.bars {
  display: none;
}
.nav_bar ul {
  display: flex;
  text-decoration: none;
  list-style: none;
}
.nav_bar ul li a {
  display: block;
  color: var(--blanco);
  font-size: 18px;
  padding: 10px 25px;
  border-radius: 15px;
  transition: 0.2s;
  margin: 0 5px;
  text-decoration: none;
}
.nav_bar ul li a:hover {
  background-color: var(--azul_oscuro);
}
.nav_bar ul li a.active {
  background-color: var(--azul_oscuro);
}
@media (max-width: 900px) {
  .header {
    padding: 0 30px;
  }
  .bars {
    display: block;
    cursor: pointer;
  }
  .bars .line {
    width: 30px;
    height: 3px;
    background-color: var(--blanco);
    margin: 6px 0;
  }
  .nav_bar {
    height: 0px;
    position: absolute;
    top: 80px;
    left: 0;
    right: 0;
    width: 100vw;
    background-color: var(--gris);
    transition: 0.5s;
    overflow: hidden;
  }
  .nav_bar.active {
    height: 450px;
  }
  .nav_bar ul {
    display: block;
    width: fit-content;
    margin: 80px auto 0 auto;
    text-align: center;
    transition: 0.5s;
    opacity: 0;
  }
  .nav_bar.nav_bar.active ul {
    opacity: 1;
  }
  .nav_bar ul li a {
    margin-bottom: 20px;
  }
}
</style>