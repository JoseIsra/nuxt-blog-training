<template>
  <div class="w-full h-full flex flex-col items-center justify-center my-20">
    <section class="w-[18rem] p-8 border border-purple-400 rounded-md">
      <p class="font-semibold text-gray-800 text-2xl md:text-3xl">Login</p>
      <form @submit.prevent="handleSubmitLogin" class="flex flex-col gap-5">
        <div>
          <label class="text-gray-600 text-sm md:text-lg">Correo</label>
          <input
            v-model="email"
            autofocus
            class="p-3 w-full border border-gray-600 text-sky-950 outline-none rounded-md"
          />
        </div>
        <div>
          <label class="text-gray-600 text-sm md:text-lg"> Contraseña </label>
          <input
            v-model="password"
            class="p-3 w-full border border-gray-600 text-sky-950 outline-none rounded-md"
          />
        </div>
        <div>
          <button
            type="submit"
            class="rounded-md border border-blue-600 bg-blue-500 py-2 px-4 outline-none w-full text-slate-300 font-semibold hover:bg-blue-400"
          >
            Iniciar sesión
          </button>
        </div>
      </form>
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

type Data = {
  email: string
  password: string
}
export default Vue.extend({
  name: 'LoginPage',
  layout: 'home',
  data(): Data {
    return {
      email: '',
      password: '',
    }
  },
  methods: {
    handleSubmitLogin() {
      this.$router.push({ name: 'home' })
    },
  },
})
</script>

<style scoped></style>
