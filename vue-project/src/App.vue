<template>
  <div>
    <h1>{{ msg }}</h1>

    <appCar></appCar>
  </div>
</template>

<script>

import Car from './Car.vue'

export default {
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    appCar: Car
  }
}
</script>

<style>

</style>
