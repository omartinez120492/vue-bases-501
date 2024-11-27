<template>
  <div class="container ">
  <!-- <UserApp  :listPersons="listaPersonas" /> -->
  <PostApi></PostApi>

  </div>
</template>

<script setup>

import PostApi from './posts/PostApi.vue';
import UserApp from './users/UserApp.vue';

const listaPersonas = [{
  nombre: 'Kiko',
  descripcion: ' Persona que es de cierta forma',
  foto: 'https://static.vecteezy.com/system/resources/previews/000/439/863/non_2x/vector-users-icon.jpg'
},
{
  nombre: 'El chavo',
  descripcion: ' Persona que es de cierta forma',
  foto: 'https://static.vecteezy.com/system/resources/previews/000/439/863/non_2x/vector-users-icon.jpg'
},
{
  nombre: 'Don Ramon',
  descripcion: ' Persona que es de cierta forma',
  foto: 'https://static.vecteezy.com/system/resources/previews/000/439/863/non_2x/vector-users-icon.jpg'
}]


</script>
<style>
</style>