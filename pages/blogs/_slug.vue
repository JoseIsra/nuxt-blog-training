<template>
  <div>
    esto es un slug= {{ $route.params.slug }}
    <div>
      <vue-markdown>
        {{ demo }}
      </vue-markdown>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import VueMarkdown from 'vue-markdown'
export default Vue.extend({
  name: 'BlogPage',
  components: { VueMarkdown },
  data() {
    return {
      mySlug: this.$route.params.slug,
      demo: `
      # Encabezado macizo
      `,
    }
  },
  head() {
    return {
      title: this.$route.params.slug,
      meta: [{ name: 'description', content: this.$route.params.slug }],
    }
  },
})
</script>

<style scoped></style>
