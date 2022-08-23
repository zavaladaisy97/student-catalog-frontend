<script>
// import axios from "axios";

export default {
  data: function () {
    return {
      message: "Welcome to the Student Catalog!",
      students: [{ first_name: "Bob", last_name: "Jones", capstone_name: "How to train your dragon" }],
    };
  },
  created: function () {
    //   this.indexStudents();
  },
  methods: {
    // indexStudents: function () {
    //   axios.get("/students.json").then((response) => {
    //     this.students = response.data;
    //     console.log("All Students", response.data);
    //   });
  },
};
</script>

<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <div v-for="student in students" v-bind:key="student.first_name">
      <h2>{{ student.first_name }}</h2>
      <p>{{ student.capstone_name }}</p>
    </div>
  </div>
</template>

<style></style>
