<script>
export default {
  data: () => ({
    title: "",
    genre: ""
  }),
  methods: {
    submitCard() {
      this.$emit('add-card', this.title, this.genre)
    }
  }
}
</script>

<template>
  <div class="NewCard">
    <h3>Add Show</h3>
    <label>Title: </label>
    <input v-model="title" />
    <label>Genre: </label>
    <input v-model="genre" />
    <button @click="submitCard">Submit</button>
  </div>
</template>

<style scoped>
div {
  background-color: #ED7063;
  border-radius: 10px;
  box-shadow: 0 2px 2px 0 rgba(0,0,0,0.16);
  color: white;
  display: inline-block;
  margin: 0 20px 20px 0;
  padding: 5px 30px 30px 30px;
  width: 200px;
}

label {
  display: block;
  margin: 10px 0 5px 0;
}

button {
  margin-top: 18px;
  padding: 8px 10px;
}
</style>
