<template>
    <div>
        <p>Trạng thái {{ status  }}</p>
        <button @click="changeStatus">Thay đổi trạng thái</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const status = ref("Online");


const changeStatus = () => {
    if (status.value == "Online"){
        status.value  = "Offline";
    } else {
        status.value = "Online";
    }
}
</script>

<style lang="scss" scoped>

</style>