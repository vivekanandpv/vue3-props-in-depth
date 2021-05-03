<template>
  <div>
    <h3>Container Component</h3>
    <hr />
    <!-- static props do not use v-bind or : shortcut -->
    <Card
      :firstName="dataFirstName"
      :lastName="dataLastName"
      :isActive="dataIsActive"
      :year="dataYear"
      :cities="dataCities"
    />
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
      dataIsActive: true,
      dataYear: "2021", //  This is ok now as number or string is taken,
      dataCities: ["Chennai", "Mysuru", "Haveri"],
    };
  },
};
</script>

<style>
</style>