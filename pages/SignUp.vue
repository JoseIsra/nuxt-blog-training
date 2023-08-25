<template>
  <div class="w-full h-full flex flex-col items-center justify-center my-20">
    <div class="border border-blue-500 rounded-md p-8 w-[20rem]">
      <p class="text-gray-800 text-2xl md:text-3xl font-semibold">Registrate</p>
      <form class="p-3 flex flex-col gap-5">
        <div>
          <label class="text-gray-600 text-sm md:text-lg">Nombre</label>
          <input
            v-model="userName"
            class="outline-none rounded-md border border-gray-600 text-sky-950 p-3 w-full"
          />
        </div>
        <div>
          <label class="text-gray-600 text-sm md:text-lg">Correo</label>
          <input
            v-model="email"
            class="outline-none rounded-md border border-gray-600 text-sky-950 p-3 w-full"
          />
        </div>
        <div>
          <label class="text-gray-600 text-sm md:text-lg"> Contraseña </label>
          <input
            v-model="password"
            class="outline-none rounded-md border border-gray-600 text-sky-950 p-3 w-full"
          />
        </div>
        <div>
          <button
            class="rounded-md border border-blue-600 bg-blue-500 py-2 px-4 outline-none w-full text-slate-300 font-semibold hover:bg-blue-400"
          >
            Iniciar sesión
          </button>
        </div>
      </form>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

type Data = {
  email: string
  userName: string
  password: string
}
export default Vue.extend({
  name: 'SignUpPage',
  layout: 'home',
  data(): Data {
    return {
      email: '',
      userName: '',
      password: '',
    }
  },
})
</script>

<style scoped></style>
