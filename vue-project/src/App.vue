<template>
  <div>
    <h1>Car: {{ carName }}</h1>

    <Counter 
      :counter="counter"
    ></Counter>

    <appCar 
      :carName="carName"
      :carYear="carYear"
      :counter="counter"
      :changeFunc="changeNameToAudi"
      @nameChanged="carName = $event"
      @updateCounter="counter = $event"
    ></appCar>
  </div>
</template>

<script>

import Car from './Car.vue'
import Counter from './Counter.vue'

export default {
  data () {
    return {
      carName: 'Tesla',
      carYear: 2018,
      counter: 0
    }
  },

  methods: {
    changeNameToAudi() {
      this.carName = 'Audi';
    }
  },

  components: {
    appCar: Car,
    Counter
  }
}
</script>

<style>

</style>
