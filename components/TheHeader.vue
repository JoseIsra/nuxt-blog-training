<template>
  <header class="bg-slate-200">
    <nav class="w-full p-5 flex justify-between">
      <aside>
        <nuxt-link to="/">
          <span>BLOG</span>
        </nuxt-link>
      </aside>
      <aside>
        <ul class="flex justify-evenly items-center gap-5">
          <li class="cursor-pointer hover:text-sky-500 hover:font-bolder">
            <NuxtLink to="/login">Login</NuxtLink>
          </li>
          <li class="cursor-pointer hover:text-sky-500 hover:font-bolder">
            <nuxt-link to="/signup"> Registrarse </nuxt-link>
          </li>
        </ul>
      </aside>
    </nav>
  </header>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'TheHeader',
})
</script>

<style scoped></style>
