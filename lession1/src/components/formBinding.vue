<template>
    <div>
        <div>
            <form action="">
                <div>
                    <label for="">Email</label>
                    <input type="text" v-model="email">
                </div>
                <div>
                    <label for="">Contact</label>
                    <textarea name="" id="" v-model="contact"></textarea>
                </div>

                <div>
                    <label for="">Checkbox</label>
                    <input type="checkbox" v-model="isChecked">
                </div>
            </form>
            <p>{{ email }}</p>
            <p>{{ contact }}</p>
            <p>{{ isChecked }}</p>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const email = ref("");
const contact = ref("");
const isChecked = ref("");
</script>

<style lang="scss" scoped></style>