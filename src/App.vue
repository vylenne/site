<template>
  <div class="app">
    <Menu/>
    <router-view class="content"/>
  </div>
</template>

<script>
import Menu from '@/components/Menu.vue';

export default {
  components: {
    Menu,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Spartan:wght@400;600&family=Syne:wght@700&display=swap');
body, p {
  margin: 0;
}

.app {
  display: flex;
  height: 100vh;
  color: #1D1D1D;
}

.content {
  box-sizing: border-box;
  padding: 40px 0;
}
</style>
