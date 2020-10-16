<script>
export default {
  data: () => ({
    counter: 0
  })
}
</script>

<template>
  <div className="Counter">
    <h3>{{counter}}</h3>
    <button @click="counter--">-</button>
    <button @click="counter++">+</button>
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
}

.Counter button {
  height: 30px;
  width: 30px;
}

</style>
