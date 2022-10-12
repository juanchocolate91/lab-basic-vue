<template>
  <h2>Ejercicio-cambiar-background</h2>
  <div :class="hola ? 'iteracion3' : 'turnOff'"></div>
  <div>
    <button @click="cuadroAzul">click me</button>
  </div>
  <h2>Ejercicio-v-show</h2>
  

  <div v-if="vShow" class="cuadro-pur">
  </div>
  <button @click="aparecer">Show purple box</button>
</template>
<script setup>
import { ref } from "vue";

const hola = ref(true);
const cuadroAzul = () => (hola.value = !hola.value);

const vShow = ref(true);
const aparecer = () => (vShow.value = !vShow.value);
</script>

<style scoped>
.iteracion3 {
  background-color: blue;
  width: 50px;
  height: 50px;
}
.turnOff {
  background-color: orange;
  width: 50px;
  height: 50px;
}
.cuadro-pur {
  background-color: blueviolet;
  width: 50px;
  height: 50px;
}
</style>
