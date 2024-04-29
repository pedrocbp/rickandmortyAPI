<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  name: String,
  status: String,
  species: String,
  gender: String,
  location: String,
  image: String,
  episodeCount: Number
});
</script>

<template>
  <div class="col-md-4">
    <div class="card mb-3">
      <img :src="props.image" class="card-img-top" alt="Imagem do personagem">
      <div class="card-body">
        <h5 class="card-title">{{ props.name }}</h5>
        <p class="card-text"><strong>Status:</strong> {{ props.status }}</p>
        <p class="card-text"><strong>Espécie:</strong> {{ props.species }}</p>
        <p class="card-text"><strong>Gênero:</strong> {{ props.gender }}</p>
        <p class="card-text"><strong>Localização Atual:</strong> {{ props.location }}</p>
        <p class="card-text"><strong>Quantidade de Episódios:</strong> {{ props.episodeCount }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped>

.card-body{
    margin-bottom: 20px;
}
</style>
