<template>
    <div>
      <h3>Student Component</h3>
      <button @click="sendStudentInfo">Kirim Data Mahasiswa</button>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      sendStudentInfo() {
        const student = { name: 'John Doe', major: 'Computer Science' };
        this.$emit('student', student);
      },
    },
  };
  </script>
  