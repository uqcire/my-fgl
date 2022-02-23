<script lang="ts" setup>
'FullWidthImage';

import { defineProps } from 'vue';

const props = defineProps({
  imgUrl: { type: String, default: '' },
  imgAlt: { type: String, default: '' },
});
</script>

<template>
  <section id="layout-background-image" class="col-span-12">
    <div class="fgl-background">
      <picture>
        <img :src="imgUrl" :alt="imgAlt" />
      </picture>
      <slot />
    </div>
  </section>
</template>
