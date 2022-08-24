<script>
import axios from "axios";

export default {
  data: function () {
    return {
      student: { first_name: "Bob", last_name: "Jones", capstone_name: "How to train your dragon", id: 1 },
    };
  },
  created: function () {
    this.showStudent();
  },
  methods: {
    showStudent: function () {
      axios.get(`/students/${this.$route.params.id}.json`).then((response) => {
        this.student = response.data;
        console.log("One Student", this.student);
      });
    },
  },
};
</script>

<template>
  <div class="home">
    <h1>{{ student }}</h1>
    <a href="/studentcatalog">Back To All Students</a>
  </div>
</template>

<style></style>
