<template>
  <div>
    <!-- header -->
    <Navbar :options="options" />
    <Nuxt class="min-h-screen" />
    <!-- footer -->
    <TheFooter />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'MainLayout',
  data(): {
    options: Array<string>
  } {
    return {
      options: ['Web', 'Videojuegos', 'FRONTEND', 'BACKEND', 'Articulos'],
    }
  },
})
</script>
