<script>
import Card from "./Card";

export default {
  components: {
    Card,
  },
  data: () => ({
    cards: [
      { title: "Rick & Morty", genre: "Animation" },
      { title: "Peaky Blinders", genre: "Drama" },
    ],
  }),
};
</script>

<template>
  <h2>Cards</h2>
  <Card
    v-for="card in cards"
    :key="card.title"
    :title="card.title"
    :genre="card.genre"
  />
</template>
