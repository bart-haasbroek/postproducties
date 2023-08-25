<script lang="ts" setup>
import Lightgallery from "lightgallery/vue/LightGalleryVue.umd.js";

import lgVideo from "lightgallery/plugins/video/lg-video.umd.js";

const plugins = [lgVideo];

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
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-21-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-21-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
  {
    url: "05-16-2018-Marianne-12-2000x1200.jpg",
    thumb: "05-16-2018-Marianne-12-2000x1200.jpg",
  },
]);
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-4 xl:grid-cols-5"
      :settings="{ speed: 500, plugins: plugins }"
    >
      <a
        data-lg-size="1280-720"
        data-src="//www.youtube.com/watch?v=EIUJfXk3_3w"
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        data-sub-html="<h4>Puffin Hunts Fish To Feed Puffling | Blue Planet II | BBC Earth</h4><p>On the heels of Planet Earth II's record-breaking Emmy nominations, BBC America presents stunning visual soundscapes from the series' amazing habitats.</p>"
      >
        <img
          width="300"
          height="100"
          class="img-responsive"
          src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        />
      </a>
      <a
        data-lg-size="1280-720"
        data-src="/videos/raindrops.mp4"
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        data-sub-html="<h4>Puffin Hunts Fish To Feed Puffling | Blue Planet II | BBC Earth</h4><p>On the heels of Planet Earth II's record-breaking Emmy nominations, BBC America presents stunning visual soundscapes from the series' amazing habitats.</p>"
      >
        <img
          width="300"
          height="100"
          class="img-responsive"
          src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        />
      </a>
    </Lightgallery>
    <!-- <Lightgallery class="grid grid-cols-4 xl:grid-cols-5">
      <a v-for="{ url, thumb } of images" :data-src="`/images/${url}`">
        <img class="img-responsive" :src="`/images/${thumb}`" />
      </a>
    </Lightgallery> -->
  </div>
</template>
