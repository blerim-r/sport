<template>
  <div class="link-container flex flex-align-center">
    <div class="flex">
      <a href="javascript:" class="no-a-style">Regolamento</a>
      <a href="javascript:" class="no-a-style">Gioco responsabile</a>
      <a href="javascript:" class="no-a-style">Privacy policy</a>
      <a href="javascript:" class="no-a-style">Termini e condizioni</a>
      <a href="javascript:" class="no-a-style">Contatti</a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "TopLinksComponent"
  }
</script>

<style scoped lang="scss">
  @import "../assets/scss/const";

  .link-container {
    background-color: #373f46;
    box-shadow: inset -4px -6px 10px rgba(0, 0, 0, 0.5);
    height: 35px;
    a {
      font-size: 0.7em;
      color: #fff;
      font-family: $top-nav-font-family;
      font-weight: 700;
      text-transform: uppercase;
      &:not(:first-child) {
        margin-left: 25px;
    }
    }
  }
</style>