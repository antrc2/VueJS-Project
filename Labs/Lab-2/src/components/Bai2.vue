<template>
    <div class="container">
        <h1>Quản lí thông tin người dùng với reactive()</h1>
        <form @submit.prevent="submitForm" action="">
            <label for="">Tên: <input type="text" v-model="user.name" required></label>
            <label for="">Tuổi: <input type="number" v-model="user.age" required></label>
            <label for="">Email: <input type="email" v-model="user.email" required></label>
            <button type="submit">Cập nhật</button>
            
        </form>
    </div>
</template>

<script setup>
import { reactive } from 'vue';

const user = reactive({
    name: "",
    age: null,
    email: "",
})

const submitForm = () => {
    if (user.name && user.email){
        alert("Thông tin hợp lệ")
    } else {
        alert("Thông tin không hợp lệ")
    }
}
</script>

<style lang="scss" scoped>

</style>