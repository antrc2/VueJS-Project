<template>
    <div>
        <h1>{{ message }}</h1>
        <button v-on:click="handleChange">ChangeMessage</button>
    </div>
</template>

<script setup>
import { onMounted, onUnmounted, onUpdated, ref } from 'vue';

const handleChange = () => {
    message.value = "Life Cycle";
}

const message = ref("Hello World!");
console.log("mounted");

onMounted(() => {
    console.log("onmounted");
})
onUpdated(() => {
    console.log("updated")
})

onUnmounted(() => {
    console.log("unmounted");
})

console.log("created");
</script>

<style lang="scss" scoped></style>