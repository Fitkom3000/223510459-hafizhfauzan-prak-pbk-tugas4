<template>
    <div>
      <h2>Child Component</h2>
      <StudentComponent @student="passStudentInfo" />
    </div>
  </template>
  
  <script>
  import StudentComponent from './StudentComponent.vue';
  
  export default {
    components: {
      StudentComponent,
    },
    methods: {
      passStudentInfo(data) {
        this.$emit('student-info', data);
      },
    },
  };
  </script>
  