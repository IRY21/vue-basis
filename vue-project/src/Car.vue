<template>
    <div>
        <slot name="title"></slot>

        <hr>
        <hr>

        <slot name="text"></slot>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
div {
  padding: 10px;
  border: 1px solid #000;
}
h2 {
  color: red;
}
</style>
