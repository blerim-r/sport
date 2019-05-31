<template>
  <div class="app-container">
    <match-container-component />
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
    padding: 50px 0;
    background-color: $body-bg;
    min-height: calc(100vh - 186px);
    position: relative;
    @include backgroundImage(url(../assets/imgs/pes2011_stadium_x18_bmp_jpgcopy.png));
    background-position: center;
    background-repeat: no-repeat;
    @include backgroundSize(contain);
  }
</style>
