<template>
  <div>
    <!-- header -->
    <TheHeader />
    <Nuxt />
    <!-- footer -->
    <TheFooter />
  </div>
</template>
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'HomeLayout',
})
</script>
