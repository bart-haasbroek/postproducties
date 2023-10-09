<script lang="ts" setup>
import Lightgallery from "lightgallery/vue/LightGalleryVue.umd.js";
import lgVideo from "lightgallery/plugins/video/lg-video.umd.js";
const plugins = [lgVideo];
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-1 md:grid-cols-2 2xl:grid-cols-3"
      :settings="{ speed: 500, plugins: plugins }"
    >
      <a
        data-video='{"source": [{"src":"/videos/1 - Plein10-2022_DEF.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb0-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb01-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/2 - Landal campagne Waterparken_V10.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb02-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb02-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/3 - VCL@SEA_DEF 1m.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb03-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb03-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/3.1 - SALTO-Familie video_07.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb3.1-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb3.1-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/3.2 - Salto Interview_def-ENG-nieuw-klein2.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb07-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb07-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/4 -1920x1080-NL- TITANIC - Landal Valentijns campnge_DEF.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb04-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb04-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/5 - BVM - Tompoezenfestival_aftrap_DEF.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb05-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb05-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/6 - SSR23 - After Movie.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb06-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb06-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/videos/8 - His Glory Reveald_DEF-klein2.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true, "loop": true}}'
        data-poster="/images/thumbs/thumb08-900x500.png"
        class="img-responsive w-full h-full object-cover object-top relative cursor-pointer group"
      >
        <img src="/images/thumbs/thumb08-900x500.png" />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

    </Lightgallery>
  </div>
</template>
