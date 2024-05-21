<template>
  <div>
    <ParentComponent>
      <h2>Data Mahasiswa</h2>
      <p>Nama: Jane Smith</p>
      <p>Jurusan: Teknik Informatika</p>
    </ParentComponent>
  </div>
</template>

<script>
import ParentComponent from './components/ParentComponent.vue';

export default {
  components: {
    ParentComponent,
  },
};
</script>
