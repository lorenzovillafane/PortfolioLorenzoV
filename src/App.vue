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
  <main>
    <router-view></router-view>
  </main>

</template>
<style>
body{background-color: #EBE3D5;}
main{
  display: flex;
  justify-content: center;
  flex-direction: column;
}</style>
