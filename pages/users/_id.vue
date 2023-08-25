<template>
  <div>
    <h1>Detalle de usuario {{ $route.params.id }}</h1>
    <nuxt-link to="/">Volver al INICIO</nuxt-link>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'UserDetail',
})
</script>

<style scoped></style>
