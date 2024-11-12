<template>
    <div class="container">
        <h1>One-way và Two-way Binding</h1>
        <p>One-way binding: <input type="text" :value="message" readonly></p>
        <p>Two-way binding: <input type="text" v-model="message"></p>
        <p>Giá trị hiện tại: {{ message }}</p>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const message = ref("Xin chào")
</script>

<style lang="scss" scoped>

</style>