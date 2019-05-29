<template>
  <div id="app">
    <top-links-component />
    <nav-links-component />
    <router-view/>
    <footer-component />
  </div>
</template>

<style lang="scss">

</style>
<script>
  import TopLinksComponent from "./components/TopLinksComponent";
  import NavLinksComponent from "./components/NavLinksComponent";
  import FooterComponent from "./components/FooterComponent";
  import "./assets/scss/app.scss";

  export default {
    components: {FooterComponent, NavLinksComponent, TopLinksComponent}
  }
</script>