<template>
  <div class="p-5 rounded-m w-full">
    <div>
      <figure class="w-[200px] h-[200px]">
        <img :src="src" :alt="alt" class="w-full h-auto object-contain" />
      </figure>
    </div>
    <div>
      <p>{{ title }}</p>
      <p>{{ subtitle }}</p>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'BCard',
  props: {
    src: {
      type: String,
      default: '',
    },
    alt: {
      type: String,
      default: '',
    },
    title: {
      type: String,
      default: '',
    },
    subtitle: {
      type: String,
      default: '',
    },
  },
})
</script>

<style scoped></style>
