<script>
export default {
  data: function () {
    return {
      message: "Welcome to Vue.js!",
      message2: "This is a test!",
      message3: "this is the one i changed!",
    };
  },
  created: function () {},
  methods: {},
};
</script>

<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <h2>{{ message2 }}</h2>
    <h3>{{ message3 }}</h3>
  </div>
</template>

<style></style>
