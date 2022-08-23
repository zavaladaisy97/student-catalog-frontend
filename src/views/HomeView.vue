<script>
export default {
  data: function () {
    return {
      message: "Welcome to Vue.js!",
      message2: "This is a test!",
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
  </div>
</template>

<style></style>
