<template>
  <div>
    <h1>Car: {{ carName }}</h1>

    <appCar 
      :carName="carName"
      :carYear="carYear"
    ></appCar>
  </div>
</template>

<script>

import Car from './Car.vue'

export default {
  data () {
    return {
      carName: 'Tesla',
      carYear: 2018
    }
  },
  components: {
    appCar: Car
  }
}
</script>

<style>

</style>
