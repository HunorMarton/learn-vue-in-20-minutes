<script>
export default {
  data: () => ({
    counter: 0
  }),
  methods: {
    decrease() {
      this.counter--
    },
    increase() {
      this.counter++
    }
  }
}
</script>

<template>
  <div>
    <h3>{{counter}}</h3>
    <button @click="decrease">-</button>
    <button @click="increase">+</button>
  </div>
</template>

<style scoped>
div {
  background-color: #ED7063;
  border-radius: 10px;
  box-shadow: 0 2px 2px 0 rgba(0,0,0,0.16);
  color: white;
  display: inline-block;
  padding: 10px 15px 20px 15px;
  text-align: center;
  width: 100px;
}

button {
  height: 30px;
  width: 30px;
}
</style>
