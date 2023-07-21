<script setup>
import Header from "./components/Header.vue";
</script>

<template>
  <div>
    <Header />
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

</style>
