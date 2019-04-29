<template>
  <div id="app">
    <Navigation></Navigation>
    <img class="logo" src="./assets/logo.png">
    <router-view/>
    <img class="graph" src="./assets/graphs.jpg">
  </div>
</template>

<script>
import Navigation from "./components/Navigation";

export default {
  name: "app",
  components: {
    Navigation
  }
};
</script>

<style>
#app {
  font-family: HeadlineBlack, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #512b2b;
  /* margin-top: 60px; */
}

.logo {
  height: 100px;
  width: 100px;
  padding-top: 100px;
}
</style>
