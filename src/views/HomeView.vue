<script setup>
import { onMounted, reactive, ref } from 'vue';
import ListCharacters from '../components/ListCharacters.vue';

let characters = reactive(ref([]));

onMounted(() => {
  fetch("https://rickandmortyapi.com/api/character?page=2")
  .then(response => response.json())
  .then(data => {
    characters.value = data.results.map(character => {
      character.episodeCount = character.episode.length;
      return character;
    });
    console.log(characters);
  })
})
</script>

<template>
  <main>
    <div class="container">
      <div class="row mt-4">
        <ListCharacters
          v-for="character in characters"
          :key="character.id"
          :name="character.name"
          :status="character.status"
          :species="character.species"
          :gender="character.gender"
          :location="character.location.name"
          :image="character.image"
          :episodeCount="character.episodeCount" 
        />
      </div>
    </div>
  </main>
</template>

<style scoped>



</style>
