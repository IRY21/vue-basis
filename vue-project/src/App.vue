<template>
  <div>
    <Counter></Counter>

    <appCar></appCar>
  </div>
</template>

<script>
import Car from './Car.vue'
import Counter from './Counter.vue'

export default {
  components: {
    appCar: Car,
    Counter
  }
}
</script>

<style>

</style>
