<script setup>

  import { ref } from 'vue';

  //Variables
  const nombre  = "ProderDev"
  const anio = 2026
  const precioBase = 78
  const iva = 21
  const coche = 
  {
    "marca": "Lamborghini",
    "modelo" : "SVJ",
    "kilometros" : "500"
  }
  const mensaje = ref('');

</script>

<template>
  
  <p>Hola, soy {{ nombre }} y estamos en {{ anio }}</p>

  <p>Si al precio de {{ precioBase }}€ le hacemos un {{ iva }}% se nos queda en un {{ (precioBase - (precioBase * iva) / 100) }}</p>

  <p>Tenemos en stock un {{ coche.marca }} de modelo {{ coche.modelo }}, con tan solo {{ coche.kilometros }}km.</p>

  <input type="text" v-model="mensaje">
  <p>Has escrito {{ mensaje }}</p>
</template>

<style scoped>

</style>