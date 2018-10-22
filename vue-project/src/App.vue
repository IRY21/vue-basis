<template>
  <div>
    <h1>Car: {{ carName }}</h1>

    <appCar 
      :carName="carName"
      :carYear="carYear"
      :changeFunc="changeNameToAudi"
      @nameChanged="carName = $event"
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

  methods: {
    changeNameToAudi() {
      this.carName = 'Audi';
    }
  },

  components: {
    appCar: Car
  }
}
</script>

<style>

</style>
