<template>
  <div id="app">
    <Navbar />
    <Steps></Steps>
    <PatientInfo></PatientInfo>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Steps from './components/Steps.vue';
import PatientInfo from './components/PatientInfo.vue';

export default {
  name: 'app',
  components: {
    Navbar,
    Steps,
    PatientInfo
  }
};
</script>

<style>
#app {
  font-family: "Helvetica65", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #162d3d;
  height: 100vh;
  background: #f3f6f9;
}
h1 {
  font-size: 36px;
  color: #162d3d;
}
.custom-input {
  height: 60px !important;
  z-index: 9;
  border: 1px solid #c1e4fe !important;
  border-top-left-radius: 6px !important;
  border-bottom-left-radius: 6px !important;
  padding: 0 48px 2px 24px !important;
  display: -ms-flexbox;
  display: flex;
  margin: 0 -1px 0 0;
  -ms-flex-pack: center;
  justify-content: center;
  font-size: 20px;
  width: 100%;
  position: relative;
}
.sub-header {
  font-size: 15px;
  margin-top: 20px;
  line-height: 18px;
  color: #32536a;
  text-align: left;
}
.btn-next {
  padding: 0 30px !important;
  border-radius: 30em !important;
  height: 42px;
  background: #3899ec !important;
  border: 1px solid #3899ec !important;
  outline: none;
  float: right;
}
</style>
