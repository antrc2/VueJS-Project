<template>
    <div class="container mt-5">
        <form action="" v-if="!isLoggedIn" class="p-4 border rounded bg-light">
            <div class="form-group">
                <label for="username">Tài khoản</label>
                <input type="text" id="username" class="form-control" placeholder="Nhập tài khoản">
            </div>
            <div class="form-group">
                <label for="password">Mật khẩu</label>
                <input type="password" id="password" class="form-control" placeholder="Nhập mật khẩu">
            </div>
            <div>
                <button class="btn btn-primary w-100">Đăng nhập</button>
            </div>
        </form>
        <div v-else class="text-center">
            <h1 class="mt-5">Chào mừng {{ username }} đã xuất hiện</h1>
        </div>
    </div>
</template>

<script setup>

import { ref } from 'vue';

// const isLoggedIn = ref(false);

const isLoggedIn = ref(true);
const username = ref("Nguyễn Ngọc An");

</script>

<style lang="scss" scoped>

</style>