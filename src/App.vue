<template>
    <div id="app">
        <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
        <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
        <headerComponent/>
        <contentComponent/>
        <footerComponent/>
    </div>
</template>

<script>
import headerComponent from "./components/Header.vue";
import footerComponent from "./components/Footer.vue";
import contentComponent from "./components/Content.vue";
export default {
  name: "app",
  components: {
    headerComponent,
    footerComponent,
    contentComponent
  }
};
</script>

<style lang="sass">
@import './assets/sass/main'
</style>
