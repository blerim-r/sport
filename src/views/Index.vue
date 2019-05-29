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

<style scoped lang="scss">
  @import "../assets/scss/const";
  @import "../assets/scss/vars";

  .app-container {
    background-color: $body-bg;
    height: 100%;
    @include backgroundImage(url(../assets/imgs/pes2011_stadium_x18_bmp_jpgcopy.png));
    background-position: center;
    background-repeat: no-repeat;
    @include backgroundSize(contain)
  }
</style>