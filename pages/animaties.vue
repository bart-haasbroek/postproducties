<script lang="ts" setup>
import Lightgallery from "lightgallery/vue/LightGalleryVue.umd.js";

import lgVideo from "lightgallery/plugins/video/lg-video.umd.js";

const plugins = [lgVideo];
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-4 2xl:grid-cols-5"
      :settings="{ speed: 500, plugins: plugins }"
    >
      <a
        data-src="//www.youtube.com/watch?v=EIUJfXk3_3w"
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
      </a>
      <a
        data-video='{"source": [{"src":"/videos/raindrops.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true}}'
        data-poster="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg"
      >
        <img src="https://img.youtube.com/vi/EIUJfXk3_3w/maxresdefault.jpg" />
      </a>
    </Lightgallery>
  </div>
</template>
