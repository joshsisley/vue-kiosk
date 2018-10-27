<template>
  <div id="app">
    <Navbar />
    <Steps></Steps>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Steps from './components/Steps.vue';

export default {
  name: 'app',
  components: {
    Navbar,
    Steps
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #162d3d;
  height: 100vh;
  background: #f3f6f9;
}
</style>
