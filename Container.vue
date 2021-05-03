<template>
  <div>
    <h3>Container Component</h3>
    <hr />
    <!-- static props do not use v-bind or : shortcut -->
    <Card firstName="Raman" lastName="Vasudev" isActive="true" year="2021" />
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