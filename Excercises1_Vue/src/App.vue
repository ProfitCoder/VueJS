<script setup>

  //Variables
  const nombre  = "ProderDev"
  const anio = 2026

  const precioBase = 78
  const iva = 21

</script>

<template>
  
  <p>Hola, soy {{ nombre }} y estamos en {{ anio }}</p>

  <p>Si al precio de {{ precioBase }}€ le hacemos un {{ iva }}% se nos queda en un {{ (precioBase - (precioBase * iva) / 100) }}</p>



</template>

<style scoped>

</style>