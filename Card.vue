<template>
  <div>
    <h4>Card Component</h4>
    <p>First Name: {{ firstName }}</p>
    <p>Last Name: {{ lastName }}</p>
    <p>Year: {{ year }}</p>
    <p>Active? {{ isActive ? "Yes" : "No" }}</p>

    <ul>
      <li v-for="(city, index) in cities" :key="index">{{ city }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    firstName: String,
    lastName: String,
    isActive: Boolean,
    year: [String, Number], //  either string or number
    cities: Array, //  array of items
  },
};
</script>

<style>
</style>