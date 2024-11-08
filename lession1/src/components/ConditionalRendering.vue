<template>
    <div>
        <h1>Conditional Rendering</h1>
        <p v-if="isActive">Active</p>
        <p v-else>Unactive</p>
    </div>
    <div>
        <p>Name: {{ user.name }}</p>
        <p v-if="user.age>=30">là trung niên</p>
        <p v-else-if="user.age=18">là thanh niên</p>
        <p v-else>là thiếu niên</p>
    </div>
</template>

<script setup>
import { reactive, ref } from 'vue';

const isActive = ref(false);
const user = reactive({
    name: "Nguyen Ngoc An",
    age: 18
})


</script>

<style lang="scss" scoped>

</style>