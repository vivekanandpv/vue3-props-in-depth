<template>
  <div>
    <h4>Card Component</h4>
    <p>First Name: {{ firstName }}</p>
    <p>Last Name: {{ lastName }}</p>
    <p>Year: {{ year }}</p>
    <p>Active? {{ isActive ? "Yes" : "No" }}</p>
  </div>
</template>

<script>
export default {
  props: {
    firstName: String,
    lastName: String,
    isActive: Boolean,
    year: Number,
  },
};
</script>

<style>
</style>