<template>
    <div>
        <div>
            <template v-for="student in students">
                <ul v-if="student.id >1" :key="student.id">
                    <li>{{ student.id }}</li>
            <li>{{ student.name }}</li>
            <li>{{ student.MSSV }}</li>
                </ul>

            </template>
        </div>
    </div>
</template>

<script setup>
import { reactive } from 'vue';

const students = reactive([
    {id: 1, name: "NNA", MSSV: "PH53674"},
    {id: 2, name: "NMT", MSSV: "PH53794"},
    {id: 3, name: "PDT", MSSV: "PH53675"}
    ])
</script>

<style lang="scss" scoped>

</style>