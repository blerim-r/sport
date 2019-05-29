<template>
  <div class="app-container">
    <match-container-component />
    <quick-links-component />
  </div>
</template>

<script>
  import MatchContainerComponent from "../components/MatchContainerComponent";
  import QuickLinksComponent from "../components/QuickLinksComponent";
  export default {
    name: "Index",
    components: {QuickLinksComponent, MatchContainerComponent}
  }
</script>

<style scoped>

</style>