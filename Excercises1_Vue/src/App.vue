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
  const mensaje = ref('')
  let ejemplo = ref('')
  const cambioSeleccionado = ref('')
  const acepta = ref('')
  const frutas =
  [
    'Manzanas',
    'Pera',
    'Naranja'
  ]

</script>

<template>
  
  <h1>Excercise 1</h1>
  <p>Hola, soy {{ nombre }} y estamos en {{ anio }}</p>

  <h1>Excercise 2</h1>
  <p>Si al precio de {{ precioBase }}€ le hacemos un {{ iva }}% se nos queda en un {{ (precioBase - (precioBase * iva) / 100) }}</p>

  <h1>Excercise 3</h1>
  <p>Tenemos en stock un {{ coche.marca }} de modelo {{ coche.modelo }}, con tan solo {{ coche.kilometros }}km.</p>

  <h1>Excercise 4</h1>
  <input type="text" v-model="mensaje">
  <p>Has escrito: {{ mensaje }}</p>

  <h1>Excercise 5</h1>
  <textarea v-model="ejemplo"></textarea>
  <p>Longitud: {{ ejemplo.length }}</p>

  <h1>Excercise 6</h1>
  <select v-model="cambioSeleccionado">
    <option selected>Albolote</option>
    <option>Granada</option>
    <option>Peligros</option>
    <option>Santafe</option>
  </select>

  <p>Ciudad elegida: {{ cambioSeleccionado }}</p>

  <h1>Excercise 7</h1>
  <input type="checkbox" v-model="acepta">

  <p>Estado: {{ acepta }}</p>

  <h1>Excercise 8</h1>

  <ol>
    <li v-for="nombre in frutas">
      {{ nombre }}
    </li>
  </ol>

</template>

<style scoped>

</style>