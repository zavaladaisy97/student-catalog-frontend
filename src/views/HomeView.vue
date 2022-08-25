<script>
export default {
  data: function () {
    return {
      message: "Welcome",
    };
  },
  created: function () {},
  methods: {},
};
</script>

<template>
  <div class="home">
    <div class="centered">
      <h1>{{ message }}</h1>
    </div>
  </div>
</template>

<style>
body {
  height: auto;
  background-size: 100%;
}

.home {
  background-image: url("https://images.unsplash.com/photo-1522071820081-009f0129c71c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80");
  display: block;
  position: absolute;
  left: 0;
  top: 15;
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: 100%;
  /* background-color: #ffffff; */
}
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  color: white;
  font-weight: bold;
  text-align: center;
  transform: translate(-50%, -50%);
}
h1 {
  font-size: 20rem !important;
}
</style>
