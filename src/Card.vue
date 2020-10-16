<script>
export default {
  props: {
    title: String,
    genre: String
  }
}
</script>

<template>
  <div class="Card">
    <h3>{{title}}</h3>
    <p>{{genre}}</p>
  </div>
</template>

<style scoped>
.Card {
  background-color: #ffffff;
  border-radius: 10px;
  box-shadow: 0 2px 2px 0 rgba(0,0,0,0.16);
  display: inline-block;
  margin: 0 20px 20px 0;
  padding: 5px 20px;
  width: 200px;
}
</style>
