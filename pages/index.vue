<script lang="ts" setup>
import Lightgallery from "lightgallery/vue/LightGalleryVue.umd.js";

function shuffle(array) {
  let currentIndex = array.length,
    randomIndex;

  // While there remain elements to shuffle.
  while (currentIndex != 0) {
    // Pick a remaining element.
    randomIndex = Math.floor(Math.random() * currentIndex);
    currentIndex--;

    // And swap it with the current element.
    [array[currentIndex], array[randomIndex]] = [
      array[randomIndex],
      array[currentIndex],
    ];
  }

  return array;
}

const images = shuffle([
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-1024x683.jpg",
  },
  {
    url: "Workshop_V1-19-2000x1200.jpg",
    thumb: "Workshop_V1-19-1024x682.jpg",
  },
  {
    url: "05-16-2018-Marianne-21-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-21-1024x683.jpg",
  },
]);
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-1 sm:grid-cols-3 md:grid-cols-4 2xl:grid-cols-5"
    >
      <a
        class="relative cursor-pointer group"
        v-for="{ url, thumb } of images"
        :data-src="`/images/${url}`"
      >
        <img class="img-responsive" :src="`/images/${thumb}`" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
    </Lightgallery>
  </div>
</template>
