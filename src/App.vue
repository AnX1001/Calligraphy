<template>
  <div id="app">
    <navBar :imgSrc="require('../src/assets/' + logo)">
      <router-link class="router-link" to="/">Home</router-link>
      <router-link class="router-link" to="/history">Historie</router-link>
      <router-link class="router-link" to="/signUp">Påmelding</router-link>
      <router-link class="router-link" to="/contact">Kontakt oss</router-link>
    </navBar>

    <router-view />
  </div>
</template>

<script>
import navBar from "@/components/navBar.vue";

export default {
  name: "App",
  components: {
    navBar,
  },
  data() {
    return {
      logo: "dragonlogo.svg",
    };
  },
};
</script>

<style lang="scss" scoped>
::v-deep * {
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  height: 100vh;

  a {
    color: white;
    text-decoration: none;
    margin-right: 10px;
    padding: 7px;
    background: black;
    font-size: 10px;
    border-radius: 3px;
    width: 68px;
    text-align: center;
  }
}
</style>
