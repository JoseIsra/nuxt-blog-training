<template>
  <header>
    <nav class="flex justify-between p-3 bg-cyan-950">
      <span class="text-slate-300 font-extrabold text-xl">BLOG</span>
      <aside>
        <label class="text-slate-300 font-bold">Usuario logeado</label>
      </aside>
    </nav>
    <nav>
      <div class="bg-cyan-800">
        <ul class="flex justify-center gap-5 p-3">
          <li
            v-for="option in options"
            :key="option"
            class="text-slate-200 hover:border-b-slate-100 hover:border-b-[1px] cursor-pointer"
          >
            {{ option }}
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script lang="ts">
import Vue, { PropType } from 'vue'

export default Vue.extend({
  name: 'BNavbar',
  props: {
    options: {
      type: Array as PropType<Array<string>>,
      default: () => [],
    },
  },
})
</script>

<style scoped></style>
