<script lang="ts" setup>
import Lightgallery from "lightgallery/vue/LightGalleryVue.umd.js";

import lgVideo from "lightgallery/plugins/video/lg-video.umd.js";

const plugins = [lgVideo];
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-1 sm:grid-cols-3 md:grid-cols-4 2xl:grid-cols-5"
      :settings="{ speed: 500, plugins: plugins }"
    >
      <a
        data-video='{"source": [{"src":"/animations/3d Pen.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/over-mij.jpg"
      >
        <img src="/images/over-mij.jpg" />
      </a>
      <a
        data-video='{"source": [{"src":"/animations/Telefoon transfer testklein.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/over-mij.jpg"
      >
        <img src="/images/05-16-2018-Marianne-12-2000x1200.jpg" />
      </a>
    </Lightgallery>
  </div>
</template>
