<script setup>
import TableComponent from '@/components/tableComponent.vue';
import { ref } from 'vue';

const students = ref([])
const message = "home view";
const deleteStudent = (id) => {
  students.value = students.value.filter((student) => student.id != id)
}
</script>

<template>
  <main>

    <TableComponent :title="message" :students="students" @delete="deleteStudent" />
  </main>
</template>