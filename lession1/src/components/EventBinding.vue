<template>
    <div>
        <button @click="count++"></button>
        <button @click="increasement">Tăng</button>
        <!-- <button @click=""></button> -->
    </div>
</template>

<script setup>
import { ref } from 'vue';

const count = ref(0);
const name = ref("NNA")
const printName = (name) => {
    alert(name)
}
const increasement = () => {
    count.value++;
}
</script>

<style lang="scss" scoped></style>