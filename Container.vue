<template>
  <div>
    <h3>Container Component</h3>
    <hr />
    <!-- see the console for errors as firstName prop is not provided -->
    <Card :lastName="dataLastName" />
  </div>
</template>

<script>
import Card from "./Card.vue";
export default {
  components: {
    Card,
  },
  //    same as data: function() {...}
  data() {
    return {
      dataFirstName: "Raman",
      dataLastName: "Vasudev",
    };
  },
};
</script>

<style>
</style>