<template>
  <div>
    <!-- <div v-if="isShow">
      <LifeCycle />
    </div> -->
    <HomeView />
    <!-- <Buoi2/> -->
    <!-- <Buoi3/> -->
    <!-- <Bai2Buoi3/> -->
    <!-- <DataBinding/> -->
    <!-- <ConditionalRendering/> -->
    <!-- <IsLogin /> -->
    <!-- <AlertForm/> -->
    <!-- <ListRendering /> -->
    <!-- <FormBinding /> -->
  </div>
</template>

<script setup>
import { ref } from 'vue';
import AlertForm from './components/alertForm.vue';
import Bai2Buoi3 from './components/Bai2Buoi3.vue';
import Buoi3 from './components/Buoi3.vue';
import ConditionalRendering from './components/ConditionalRendering.vue';
import DataBinding from './components/DataBinding.vue';
import FormBinding from './components/formBinding.vue';
import IsLogin from './components/isLogin.vue';
import LifeCycle from './components/LifeCycle.vue';
import ListRendering from './components/listRendering.vue';
import HomeView from './views/HomeView.vue';

const isShow = ref(true)

// import Buoi2 from './components/Buoi2.vue';


</script>

<style lang="scss" scoped></style>