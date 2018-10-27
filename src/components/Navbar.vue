<template>
  <b-navbar toggleable="md" type="light" class="custom-navbar">
    <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
    <b-navbar-brand href="#">Kiosk</b-navbar-brand>
  </b-navbar>
</template>

<script>
export default {
  name: 'Navbar',
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.custom-navbar {
  background: white !important;
  border-bottom: 1px solid #dfe5eb;
}
</style>
