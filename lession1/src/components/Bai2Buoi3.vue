<template>
    <div>
        <div>
            <p>Mảng: {{ total }}</p>
            <button @click="sum" >Sum</button>
        </div>
    </div>
</template>

<script setup>
import { reactive, ref } from 'vue';

const numbers = reactive([1,3,6,7,3]);
let total = ref(0)
const sum = () => {
    total.value =0;
    for (let i of numbers){
        total.value +=i;
    }
}
</script>

<style lang="scss" scoped>

</style>