<script>
import { createApp } from 'vue';
import routes from '../src/routes/routes.js';

export default {
  created() {
    createApp(this).use(routes).mount('#app');
  }
};
</script>

<template>
<router-view></router-view>
</template>
<style>
body{
  display: flex;
  justify-content: center;
}</style>
