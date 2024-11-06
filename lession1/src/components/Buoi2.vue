<template>
    <div>
        <div>
            <h1>Count: {{ person }}</h1>
            <button @click="add">Tăng</button>
        </div>

    </div>
</template>

<script setup>
import { reactive, ref } from 'vue';

let person = reactive({
    name: "John",
    age: 30
})

const add = ()=>{
    person.age++;
}
const count = reactive(0);
console.log(count)
const increment = () => {
    count++;
    console.log(count)
}


</script>

<style lang="scss" scoped>

</style>