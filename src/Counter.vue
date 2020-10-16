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
  <div className="Counter">
    <h3>{{counter}}</h3>
    <button @click="decrease">-</button>
    <button @click="increase">+</button>
    <div v-if="counter < 0">Too low</div>
  </div>
</template>

<style scoped>
.Counter {
  background-color: #ffffff;
  border-radius: 10px;
  box-shadow: 0 2px 2px 0 rgba(0,0,0,0.16);
  display: inline-block;
  padding: 5px 20px;
  text-align: center;
  height: 110px;
  width: 100px;
}

.Counter button {
  height: 30px;
  width: 30px;
}
</style>
