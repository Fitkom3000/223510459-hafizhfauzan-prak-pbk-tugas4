<template>
    <div>
      <h1>Parent Component</h1>
      <p>Data Mahasiswa: {{ studentData }}</p>
      <ChildComponent @student-info="handleStudentInfo" />
    </div>
  </template>
  
  <script>
  import ChildComponent from './ChildComponent.vue';
  
  export default {
    components: {
      ChildComponent,
    },
    data() {
      return {
        studentData: '',
      };
    },
    methods: {
      handleStudentInfo(data) {
        this.studentData = JSON.stringify(data, null, 2);
      },
    },
  };
  </script>
  