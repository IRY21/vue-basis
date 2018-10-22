<template>
  <div>
    <appCar>
      <h2 slot="title">{{ carName }} + html</h2>
      <p slot="text">Lorem, ipsum dolor.</p>
    </appCar>
  </div>
</template>

<script>
import Car from "./Car.vue";

export default {
  data() {
    return {
      carName: "Tesla"
    };
  },

  components: {
    appCar: Car
  }
};
</script>

<style scoped>
h2 {
  color: red;
}
</style>
