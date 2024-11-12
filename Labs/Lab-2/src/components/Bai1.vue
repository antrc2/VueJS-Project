<template>
    <div>
        <h1>Quản lí giỏ hàng với ref()</h1>
        <p>Số lượng sản phẩm: {{ productCount }}</p>
        <button class="btn" @click="increaseCount">Tăng</button>
        <button class="btn" @click="decreaseCount">Giảm</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const productCount = ref(0)

const increaseCount = () => {
    productCount.value++;
}

const decreaseCount = () => {
    productCount.value--
}
</script>

<style lang="scss" scoped>

</style>