<template>
  <div>
    <h3>Container Component</h3>
    <hr />
    <!-- see the console for errors as firstName prop fails validation -->
    <Card firstName="Ken" />
  </div>
</template>

<script>
import Card from "./Card.vue";
export default {
  components: {
    Card,
  },
};
</script>

<style>
</style>