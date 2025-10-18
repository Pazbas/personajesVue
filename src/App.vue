<template>
    <div>
      <p><h1>Tarea M6AE2 - ABP2</h1></p>
        </div>
        <br>
        <br>
        <br>
        <br>
     
  <div class="container">
    <h2>Lista de Personajes</h2>
    <ul>
      <li v-for="personaje in data.personajes" :key="personaje.id">
        <h2>{{ personaje.nombre }}</h2>
        <p>{{ personaje.descripcion }}</p>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

const data = reactive({
  personajes: [
    {
      id: "1",
      nombre: "pikachu",
      descripcion: "lorem ipsum uhiuhiuhihoi"
    },
    {
      id: "2",
      nombre: "kakuna",
      descripcion: "lorem ipsum uhiuhiuhihoi"
    },
    {
      id: "3",
      nombre: "beedrill",
      descripcion: "lorem ipsum uhiuhiuhihoi"
    },
    {
      id: "4",
      nombre: "metapod",
      descripcion: "lorem ipsum uhiuhiuhihoi"
    },
    {
      id: "5",
      nombre: "rattata",
      descripcion: "lorem ipsum uhiuhiuhihoi"
    }
  ]
})
</script>

<style scoped>
.container {
  max-width: 600px;
  margin: auto;
  font-family: Arial, sans-serif;
}

li {
  list-style: none;
  margin-bottom: 20px;
  border-bottom: 1px solid #ccc;
  padding-bottom: 10px;
}
</style>
