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
  <div v-for="student in students" v-bind:key="student.first_name">
    <div class="card" style="width: 18rem">
      <img
        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRaqTJE35XjsBw9H2FPMekZccFRibi7Cxqdug&usqp=CAU"
        class="card-img-top"
      />
      <div class="card-body">
        <h5 class="card-title">{{ student.first_name }} {{ student.last_name }}</h5>
        <p class="card-text">
          Bob's capstone will show you the right way to train your dragon. Click the button below to see!
        </p>
        <a class="btn btn-primary" v-bind:href="`/students/${student.id}`">Student Info</a>
      </div>
    </div>
  </div>

  <!-- <div class="home">
    <h1>{{ message }}</h1>
    <div v-for="student in students" v-bind:key="student.first_name">
      <h2>{{ student.first_name }}</h2>
      <p>{{ student.capstone_name }}</p>
      <a v-bind:href="`/students/${student.id}`">Student Info</a>
    </div>
  </div> -->
</template>

<style>
body {
  background-color: #ffffff;
}
</style>
