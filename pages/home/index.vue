<template>
  <main class="p-4 w-full bg-[#fffffe]">
    <h1 class="text-center text-3xl font-bold text-gray-800">
      Contenido del blog
    </h1>
    <div>
      <Card
        v-for="card in cards"
        :key="card.id"
        :src="card.src"
        :alt="card.alt"
        :title="card.title"
        :subtitle="card.subtitle"
        @select-card="handleCardSelected(card.title)"
      />
    </div>
  </main>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'HomePage',
  data() {
    return {
      cards: [
        {
          src: 'https://images.pexels.com/photos/261579/pexels-photo-261579.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
          alt: 'A table with notebooks, a cup of tea, a table and a pencil',
          id: 1,
          title: 'Blog Princinpal',
          subtitle:
            'Blog de BugInTheConsole donde cuenta sus experiencias y enseña lo aprendido',
        },
        {
          src: 'https://images.pexels.com/photos/12300693/pexels-photo-12300693.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
          alt: 'A young man playing a fighting game in a empty room',
          id: 2,
          title: '¿Cómo necesita un videojuego para ser bueno?',
          subtitle:
            'Debate y consideraciones sobre aspectos relevantes para un juego decente',
        },
        {
          src: 'https://images.pexels.com/photos/416405/pexels-photo-416405.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
          alt: '3 people around a table talking to each other using blueprints, calculators and more equipment',
          id: 3,
          title: 'La importancia de la gestión para un proyecto',
          subtitle:
            'Qué pasaría si no hay una correcta gestión de desarrollo de software?, ¿Qué sucede con el equipo si no hay gestión apropiada?',
        },
      ],
    }
  },
  methods: {
    handleCardSelected(titleCard: string) {
      this.$router.push({ name: 'blogs-slug', params: { slug: titleCard } })
    },
  },
})
</script>

<style scoped></style>
