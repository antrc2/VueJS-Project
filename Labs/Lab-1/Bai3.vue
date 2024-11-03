<template>
    <div>
        <h1> {{ greeting }}</h1>
    </div>
    <button :title="buttonTitle" @click="changeGreeting">Click để thay đổi</button>
</template>

<script setup>

import {ref} from "vue";

const greeting = ref("Xin chào bạn!")
const buttonTitle = ref("Nhấn vào để thay đổi lời chào")

const changeGreeting= () => {
    greeting.value = "Hello World!";
    buttonTitle.value = "Lời chào mới đã được cập nhật"
}

</script>

<style lang="scss" scoped>


</style>