<template>
  <div>
    <h4>Card Component</h4>
    <p>First Name: {{ firstName }}</p>
    <p>Last Name: {{ lastName }}</p>
  </div>
</template>

<script>
export default {
  props: {
    //    a prop now is an object
    firstName: {
      type: String,
      validator: function (value) {
        return value && value.length >= 5;
      },
      default: "Default first name as value", //  doesn't activate!
    },
    lastName: {
      type: String,
      default: function () {
        return "Default last name from function";
      },
    },
  },
};
</script>

<style>
</style>