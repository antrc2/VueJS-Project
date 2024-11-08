<template>
    <div>
        <img :src="image" alt="">
        <input type="text" v-model="image">
    </div>
</template>

<script setup>
import { ref } from 'vue';
const image = ref("https://www.rspca.org.uk/documents/d/rspca/1164739-puppy-taken-for-a-walk_3x2?imagePreview=1");
</script>

<style lang="scss" scoped>

</style>