<template>
  <div class="p-5">
    <section
      class="flex flex-col md:flex-row justify-around items-center min-h-[20rem]"
    >
      <div class="p-10">
        <p class="font-extrabold text-4xl md:text-5xl text-gray-900">
          El blog de bugInTheConsole
        </p>
      </div>
      <div>efectos cool de letras por aquí cuando se pueda aver qué sale</div>
    </section>

    <section class="my-20">
      <p class="font-medium text-xl md:text-2xl text-gray-800">
        Contenido tecnológico
      </p>
      <div
        class="flex flex-col md:flex-row gap-10 justify-around items-center p-10"
      >
        <div
          class="p-5 border rounded-md shadow-md w-full md:w-32 md:h-32 text-center"
        >
          Lectura
        </div>
        <div
          class="p-5 border rounded-md shadow-md w-full md:w-32 md:h-32 text-center"
        >
          Escritura
        </div>
        <div
          class="p-5 border rounded-md shadow-md w-full md:w-32 md:h-32 text-center"
        >
          Práctica
        </div>
        <!-- some cool cards it coold be -->
      </div>
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  layout: 'home',
})
</script>
