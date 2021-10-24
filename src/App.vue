<template>
    <router-view />
    <main-tabbar/>
</template>
<script>
import MainTabbar from './components/content/MainTabbar.vue';

export default {
  name: "app",
  components: {
    MainTabbar,
  },
};
</script>

<style>
@import "./assets/css/base.css";
</style>
