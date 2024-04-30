<script setup>
//import TheWelcome from '../components/TheWelcome.vue'
import { onMounted, reactive, ref } from 'vue';

let personagens = reactive(ref());
let types = reactive(ref());

onMounted(() => {
  fetch("https://rickandmortyapi.com/api/character?limit=60&offset=0")
  .then(response => response.json())
  .then(response => {
    personagens.value = response.results;
    console.log(personagens);
  })
})

</script>

<template>
  <div class="container">
  <div class="row">
          <div class="col-md-6" v-for="personagem in personagens" :key="personagem.id">
                <div class="card mb-3" style="max-width: 700px;">
                    <div class="row g-0 p-2 ">
                        <div class="col-md-4">
                            <img :src="personagem.image" class="card-img-top" height="100%" alt="...">
                        </div>
    <div class="col-md-8">
      <div class="card-body">
        <h5 class="card-title">{{ personagem.name }}</h5>
        <p class="card-text">Status: {{ personagem.status }}</p>
        <p class="card-text">Espécie: {{ personagem.species }}</p>
        <p class="card-text">Gênero: {{ personagem.gender }}</p>
        <p class="card-text">Episodios: {{ personagem.episode.length }}</p>
        <p class="card-text"><small class="text-body-secondary">Localização atual: {{ personagem.location.name }}</small></p>
      </div>
    </div>
  </div>
</div>
    </div>
  </div>
</div>
  </template>

<style>
.container {
  padding-top: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
  
