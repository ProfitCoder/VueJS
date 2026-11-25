<script>
  import { ref } from 'vue';

  export default {
    // `setup` is a special hook dedicated for the Composition API.
    setup() {

      //ref para que se actualice a tiempo real la variable
      //const count = ref(0)
      const nombre = ref('')
      const listaNombres = ref([]);
      //Al no ser esta reactiva no le cambia el valor
      //var nombre = "Pablo";



      //Functions
      function increment()
      {
        count.value++;
        nombre = "Pepe";

        console.log(count.value);
        console.log(nombre);
      }

      function leeNombre()
      {
        listaNombres.value.push(nombre.value);
        nombre.value = "";
      }




      // expose the ref to the template
      return {
        nombre,
        listaNombres,
        leeNombre
      }
    }
  }
</script>

<template>

  <p>{{ count }}</p>

  <div>
    {{ nombre }}
  </div>

  <button @click="increment">Incrementar </button>

    <input v-model="nombre"/>
    <button @click="leeNombre">Añadir a la lista</button>

  <ol>
    <li v-for="nombre in listaNombres">
      {{ nombre }}
    </li>
  </ol>

</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
