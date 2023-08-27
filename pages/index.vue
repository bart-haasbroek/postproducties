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
  {
    url: "vDuijn-16-09-24-2000x1200.jpg",
    thumb: "vDuijn-16-09-24-1024x683.jpg",
  },
  {
    url: "vDuijn-16-09-39-2000x1200.jpg",
    thumb: "vDuijn-16-09-39-1024x683.jpg",
  },
  {
    url: "vDuijn-16-09-45-2000x1200.jpg",
    thumb: "vDuijn-16-09-45-1024x683.jpg",
  },
  {
    url: "vDuijn-16-09-61.jpg",
    thumb: "vDuijn-16-09-61-768x1166.jpg",
  },
  {
    url: "11-11-18-Familie-Hockx-30-2000x1200.jpg",
    thumb: "11-11-18-Familie-Hockx-30-1024x683.jpg",
  },
  {
    url: "11-11-18-Familie-Hockx-37-2000x1200.jpg",
    thumb: "11-11-18-Familie-Hockx-37-1024x683.jpg",
  },
  {
    url: "18-11-18-Juffermans-14-2000x1200.jpg",
    thumb: "18-11-18-Juffermans-14-1024x683.jpg",
  },
  {
    url: "20180502-1018DSC02504-2000x1200.jpg",
    thumb: "20180502-1018DSC02504-1024x683.jpg",
  },
  {
    url: "20180502-1206DSC02762-2000x1200.jpg",
    thumb: "20180502-1206DSC02762-1024x683.jpg",
  },
  {
    url: "AnneMarjolein-07-10-15-15-2000x1200.jpg",
    thumb: "AnneMarjolein-07-10-15-15-1024x682.jpg",
  },
  {
    url: "AnneMarjolein-07-10-15-19-2000x1200.jpg",
    thumb: "AnneMarjolein-07-10-15-19-1024x621.jpg",
  },
  {
    url: "DSC01913-2000x1200.jpg",
    thumb: "DSC01913-1024x682.jpg",
  },
  {
    url: "DSC01950-2000x1200.jpg",
    thumb: "DSC01950-1024x682.jpg",
  },
  {
    url: "DSC05636-2000x1200.jpg",
    thumb: "DSC05636-1024x682.jpg",
  },
  {
    url: "NielsvDelft22-10-8-2000x1200.jpg",
    thumb: "NielsvDelft22-10-8-1024x683.jpg",
  },
  {
    url: "Peter-van-Egmond_0010-114-2000x1200.jpg",
    thumb: "Peter-van-Egmond_0010-114-1024x682.jpg",
  },
  {
    url: "PeterElise02_10-10-15-5-2000x1200.jpg",
    thumb: "PeterElise02_10-10-15-5-1024x682.jpg",
  },
  {
    url: "Portret_Arnold-20-2000x1200.jpg",
    thumb: "Portret_Arnold-20-1024x682.jpg",
  },
  {
    url: "Workshop_V2-1-2000x1200.jpg",
    thumb: "Workshop_V2-1-1024x682.jpg",
  },

  {
    url: "08-24-2020_Christine-en-Apollo-152-2048x1365.jpg",
    thumb: "08-24-2020_Christine-en-Apollo-152-1024x683.jpg",
  },
  {
    url: "08-24-2020_Christine-en-Apollo-205-2048x1365.jpg",
    thumb: "08-24-2020_Christine-en-Apollo-205-1024x683.jpg",
  },
  {
    url: "08-24-2020_Christine-en-Apollo-223-2048x1365.jpg ",
    thumb: "08-24-2020_Christine-en-Apollo-223-1024x683.jpg",
  },
  {
    url: "08-24-2020_Christine-en-Apollo-265-2048x1365.jpg",
    thumb: "08-24-2020_Christine-en-Apollo-265-1024x683.jpg",
  },
  {
    url: "20180610-1455DSC03596-2048x1346.jpg",
    thumb: "20180610-1455DSC03596-1024x673.jpg",
  },
  {
    url: "AnneMarjolein-07-10-15-4-1024x682.jpg",
    thumb: "AnneMarjolein-07-10-15-4-2048x1363.jpg",
  },
  {
    url: "DSC08666-683x1024.jpg",
    thumb: "DSC08666-1365x2048.jpg",
  },
  {
    url: "VikingFit-02-2022-12-1024x683.jpg",
    thumb: "VikingFit-02-2022-12-2048x1365.jpg",
  },
  {
    url: "VikingFit-02-2022-119-1024x683.jpg",
    thumb: "VikingFit-02-2022-119-2048x1365.jpg",
  },
]);
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-1 sm:grid-cols-3 md:grid-cols-4 2xl:grid-cols-5"
    >
      <a
        class="relative cursor-pointer group aspect-[4/3]"
        v-for="{ url, thumb } of images"
        :data-src="`/images/${url}`"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          :src="`/images/${thumb}`"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
    </Lightgallery>
  </div>
</template>
