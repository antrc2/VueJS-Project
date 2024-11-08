<template>
    <div>
        <h1 v-if="isVisible">Đăng nhập</h1>
        <h1 v-else>Đăng xuất</h1>
        <button @click="changeStatus">Change Status</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';


let isVisible = ref(true)

const changeStatus = () => {
    isVisible.value = !isVisible.value;
}
</script>

<style lang="scss" scoped>

</style>