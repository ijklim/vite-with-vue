<template>
  <div style="margin-top:20px;">First Element is a div</div>
  <button type="button" v-bind="$attrs">
    Button as 2nd element, must use v-bind $attrs to emit default click event
  </button>
</template>

<script>
export default {
}
</script>

<style scoped>
div {
  background-color: goldenrod;
  border: 1px solid white;
  border-radius: 5px;
  margin-bottom: 10px;
  padding: 10px;
}
</style>