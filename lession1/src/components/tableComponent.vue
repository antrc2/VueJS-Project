<template>
    <h3>{{ title }}</h3>
    <table>
        <thead>
            <tr>
                <th>Id</th>
                <th>Name</th>
                <th>MSSV</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="student in students" :key="student.id">
                <td>{{ student.id }}</td>
                <td>{{ student.name }}</td>
                <td>{{ student.mssv }}</td>
                <td><button @click="ChamVaoNut(student.id)">Xoá</button></td>
            </tr>
        </tbody>
    </table>

</template>

<script setup>

defineProps(['students', 'title']);
const emit = defineEmits('delete');
const ChamVaoNut = (id) => {
    emit('delete', id)
}

</script>

<style lang="scss" scoped></style>