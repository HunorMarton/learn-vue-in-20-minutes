<script>
import Card from "./Card";
import NewCard from "./NewCard";

export default {
  components: {
    Card,
    NewCard
  },
  data: () => ({
    cards: [
      { title: "Rick & Morty", genre: "Animation" },
      { title: "Peaky Blinders", genre: "Drama" },
    ],
  }),
  methods: {
    addCard(title, genre) {
      this.cards.push({ title, genre })
    }
  }
};
</script>

<template>
  <h2>TV Shows</h2>
  <Card
    v-for="card in cards"
    :key="card.title"
    :title="card.title"
    :genre="card.genre"
  />
  <NewCard @add-card="addCard" />
</template>
