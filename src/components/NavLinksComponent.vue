<template>
  <div>
    <div class="nav-container flex flex-between flex-align-center">
      <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="219" height="29" viewBox="0 0 219 29"><g><g><image width="219" height="29" xlink:href="data:image/png;base64,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"/></g></g></svg>
      <div class="flex flex-between flex-align-center h-100 flex">
        <div class="single-link flex flex-align-center active"><a href="javascript:" class="flex flex-align-center">home</a> </div>
        <div class="single-link flex flex-align-center"><a href="javascript:" class="flex flex-align-center">sport</a> </div>
        <div class="single-link flex flex-align-center"><a href="javascript:" class="flex flex-align-center">livebetting</a> </div>
        <div class="single-link flex flex-align-center"><a href="javascript:" class="flex flex-align-center">poker</a> </div>
        <div class="single-link flex flex-align-center"><a href="javascript:" class="flex flex-align-center">casino</a> </div>
        <div class="single-link flex flex-align-center"><a href="javascript:" class="flex flex-align-center">live casino</a> </div>
        <div class="single-link flex flex-align-center"><a href="javascript:" class="flex flex-align-center">games</a> </div>
        <div class="holder-menu-ital">
          <img src="../assets/imgs/menu-circular-button.png">
          <img src="../assets/imgs/italy_(3).png">
        </div>
      </div>
    </div>
    <div class="border"></div>
  </div>
</template>

<script>
  export default {
    name: "NavLinksComponent",
    data: () => ({
    })
  }
</script>

<style scoped lang="scss">
  @import "../assets/scss/const";
  @import "../assets/scss/vars";

  .nav-container {
    padding: 0 0 1px 50px;
    background-color: $body-bg;
    height: 60px;
    &:hover {
      .single-link.active {
        transform: none;
        background-color: unset;
        box-shadow: none;
        a {
          color: $nav-links-cl;
          transform: none;
        }
      }
      .single-link:hover {
        transform: skew(-20deg);
        height: 100%;
        padding: 0 10px;
        background-color: #1d1d1d;
        box-shadow: inset 0 0 10px #000000;
        a {
          color: $nav-links-cl-active;
          transform: skew(20deg);
        }
      }
    }

    .single-link.active {
      transform: skew(-20deg);
      height: 100%;
      padding: 0 10px;
      background-color: #1d1d1d;
      box-shadow: inset 0 0 10px #000000;
      a {
        color: $nav-links-cl-active;
        transform: skew(20deg);
      }
    }

    .single-link {
      height: 100%;
      padding: 0 10px;
      @include media (cs, 0, 1200px) {
        padding: 0 7px;
      }
    }
    a {
      height: 100%;
      color: $nav-links-cl;
      font-family: $nav-font-family;
      font-size: 0.857em;
      font-weight: 400;
      text-transform: uppercase;
      text-decoration: none;
      margin: 0;
    }
    .holder-menu-ital {
      background-image: url("../assets/imgs/Layer_1.png");
      height: 100%;
      background-repeat: no-repeat;
      background-size: cover;
      width: 108px;
      display: flex;
      justify-content: center;
      align-items: center;
      & img:nth-child(1) {
        padding: 0 10px;

      }
    }
  }
  .border {
    width: 100%;
    height: 3px;
    background-image: linear-gradient(to right, #ff6000 , #ff6000, #ffb700 , #ff6000 , #ff6000);
  }
</style>
