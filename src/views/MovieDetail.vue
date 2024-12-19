<template>
  <div class="movie-detail">
    <h2>{{ movie.Title }}</h2>
    <p>{{ movie.Year }}</p>
    <img :src="movie.Poster" alt="Movie Poster" class="featured-img"/>
    <p>{{ movie.Plot }}</p>
  </div>
</template>

<script>
import {ref, onBeforeMount} from 'vue';
import {useRoute} from 'vue-router';
import env from '@/env.js'

export default {
  setup() {
    const movie = ref({});
    const route = useRoute();

    onBeforeMount(() => {
      fetch(`${env.URL_API}/?apikey=${env.apikey}&i=${route.params.id}&plot=full`)
          .then((response) => response.json())
          .then((data) => {
            movie.value = data;
          })
          .catch((error) => console.log(error));
    });

    return {
      movie
    }
  }
}
</script>

<style scoped lang="scss">
.movie-detail {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
  align-items: center;
  gap: 2rem;
  width: 89%;
  margin: 0 auto;
  margin-top: 2rem;
  padding: 16px;

  h2 {
    color: #FFF;
    font-size: 28px;
    font-weight: 600;
    margin-bottom: 16px;
  }

  .featured-img {
    display: block;
    max-width: 300px;
    margin-bottom: 16px;
    border-radius: 8px;
    transition: transform 0.3s ease-in-out;
  }

  .featured-img:hover {
    transform: scale(2);
  }

  p {
    color: #FFF;
    font-size: 18px;
    line-height: 1.6;
    letter-spacing: 1.2px;
    text-align: center;
  }
}
</style>