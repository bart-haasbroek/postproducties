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

// const videos = [
//     {
//         poster: 'https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg',
//         attr: {
//             'data-src': '//www.youtube.com/watch?v=EIUJfXk3_3w',
//             'data-poster': 'https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg'
//         },
//     }
//     {
//         poster: 'https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg',
//         attr: {
//             'data-video': '{"source": [{"src":"/videos/raindrops.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true}}',
//             'data-poster': 'https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg'
//         },
//     }
// ]
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-1 md:grid-cols-2"
      :settings="{ speed: 500, plugins: plugins }"
    >
      <a
        data-src="//www.youtube.com/watch?v=EIUJfXk3_3w"
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        class="relative cursor-pointer group"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
      <a
        data-video='{"source": [{"src":"/videos/raindrops.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        class="relative cursor-pointer group"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
      <a
        data-video='{"source": [{"src":"/videos/raindrops.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        class="relative cursor-pointer group"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
      <a
        data-video='{"source": [{"src":"/videos/raindrops.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        class="relative cursor-pointer group"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
      <a
        data-video='{"source": [{"src":"/videos/raindrops.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
        class="relative cursor-pointer group"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
    </Lightgallery>
  </div>
</template>
