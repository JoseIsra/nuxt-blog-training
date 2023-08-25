<template>
  <div>
    <h1>BIENVENIDO A LA PÁGINA PRINCIPAL DE FANS 😃</h1>
    <nuxt-link :to="{ name: 'users-id', params: { id: 'LIL-PEEP' } }"
      >Ver fan destacado</nuxt-link
    >
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'UserPage',
})
</script>

<style scoped></style>
