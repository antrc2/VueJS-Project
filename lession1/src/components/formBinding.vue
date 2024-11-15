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
                <div>
                    <label for="">Male</label>
                    <input type="checkbox" value="male" v-model="gender" name="" id="">
                </div>
                <div>
                    <label for="">female</label>
                    <input type="checkbox" value="female" v-model="gender" name="" id="">
                </div>
                <div>
                    <label for="language">Ngôn ngữ lập trình</label>
                    <select v-model="selectedLanguage" name="" id="language">
                        <option value="Javascript">Javascript</option>
                        <option value="Java">Java</option>
                        <option value="C++">C++</option>
                    </select>
                </div>
                <div>
                    <input type="radio" value="Red" id="red" v-model="favouriteColor">
                    <label for="red">Red</label>
                    <input type="radio" value="Green" id="green" v-model="favouriteColor">
                    <label for="green">Green</label>
                </div>
            </form>
            <p>{{ email }}</p>
            <p>{{ contact }}</p>
            <p>{{ isChecked }}</p>
            <p>{{ gender }}</p>
            <p>{{ selectedLanguage }}</p>
            <p>{{ favouriteColor }}</p>

        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const email = ref("");
const contact = ref("");
const isChecked = ref("");
const gender = ref([]);
const selectedLanguage = ref("");
const favouriteColor = ref();
</script>

<style lang="scss" scoped></style>