<script lang="ts" setup>
import Lightgallery from "lightgallery/vue/LightGalleryVue.umd.js";

import lgVideo from "lightgallery/plugins/video/lg-video.umd.js";

const plugins = [lgVideo];
</script>

<template>
  <div class="h-full">
    <Lightgallery
      class="grid grid-cols-1 md:grid-cols-2"
      :settings="{ speed: 500, plugins: plugins }"
    >
      <a
        data-video='{"source": [{"src":"/animations/1 - Alutech - Aluminized - logo animatie.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb1-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb1-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/2 - Telefoon transfer testklein.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb2-1536x864.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb2-1536x864.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/3 - 3d Pen.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb3-1536x866.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb3-1536x866.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/4 - Bird-3.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb4-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb4-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/5 - BonBon promo_HD.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb5-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb5-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/6 - Logo animatie dots.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb6-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb6-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/7 - De Watering_Logo lagen2.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb7-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb7-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/8 - LUMC logo.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb8-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb8-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/9 - Match cut - 01.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb9-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb9-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/10 - Match cut - 02.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb10-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb10-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>

      <a
        data-video='{"source": [{"src":"/animations/11 - google balletjes.mp4", "type":"video/mp4"}], "attributes": {"preload": true, "playsinline": true, "controls": false, "loop": true}}'
        data-poster="/images/thumbs/animation-thumb11-1536x960.png"
        class="relative cursor-pointer group"
      >
        <img
          class="img-responsive w-full h-full object-cover object-top"
          src="/images/thumbs/animation-thumb11-1536x960.png"
        />
        <div
          class="absolute w-full h-full left-0 top-0 bg-[#0c6285] opacity-0 group-hover:opacity-50 transition-all duration-300"
        ></div>
      </a>
    </Lightgallery>
  </div>
</template>
