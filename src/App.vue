<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Prueba from "./components/Prueba.vue";
</script>

<template>
  <div class="page-wrapper">
    <Header />
    <main>
      <Prueba />
      <Prueba />
      <Prueba />
    </main>
    <Footer />
  </div>
</template>

<style>
:root {
  --azul_oscuro: #3d577c;
  --blanco: #f3f3f3;
  --azul_claro: #90b4d9;
  --gris: #94a4b4;
  --morado-oscuro: #8e9cb1;
  --negro: #000;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

body {
  font-size: 1.6rem;
  font-family: "Lato", sans-serif;
  background-color: var(--gris-claro);
}
.page-wrapper {
  min-height: 100vh; /* Asegura que la altura mínima sea el 100% del viewport height */
  display: flex;
  flex-direction: column;
}

main {
  flex-grow: 1; /* Hace que el contenido principal crezca para llenar el espacio disponible */
}
</style>
