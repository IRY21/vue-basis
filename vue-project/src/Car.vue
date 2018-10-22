<template>
    <div class="car">
        <h3>Name: {{ carName }}</h3>
        <p>Year: {{ carYear }}</p>
    </div>
</template>

<script>
export default {
    props: ['carName', 'carYear']
}
</script>

<style scoped>
    .car {
        border: 1px solid #000;
    }
</style>
