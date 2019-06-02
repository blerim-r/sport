<template>
  <div>
    <quick-links-component/>
    <div class="footer-container w-100">
      <img src="../assets/imgs/Vector_Smart_Object.png">
      <span class="footer-text">© 2001-2017 bet365. All rights reserved.</span>
    </div>
    <div class="top-positioner" @click="moveToTop" v-if="toggle">
      <img src="../assets/imgs/Vector_Smart_Object5.png">
    </div>
  </div>

</template>

<script>
  import QuickLinksComponent from "./QuickLinksComponent";
  import $ from 'jquery';

  export default {
    name: "FooterComponent",
    components: {QuickLinksComponent},
    data: () => ({
      toggle: false
    }),
    methods: {
      moveToTop: function () {
        $('html, body').animate({
          scrollTop: 0
        });
      },
      checkScrollBar: function () {
        this.toggle = $(document).height() > $(window).height();
      }
    },
    mounted() {
      this.checkScrollBar();
      window.addEventListener('resize', this.checkScrollBar);
      const self = this;
      const bodyObserver = new ResizeObserver(entries => {
        self.checkScrollBar();
      });
      bodyObserver.observe(document.getElementById('app'));
    },
  }
</script>

<style scoped lang="scss">
  @import "../assets/scss/const";
  @import "../assets/scss/class";

  .footer-container {
    position: relative;
    height: 52px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    background-color: #1d1d1d;

    img {
      margin: auto;
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
    }

    span {
      color: #bbbbbb;
      font-family: $font-rajdhani;
      font-size: 14px;
      font-weight: 400;
      padding-right: 50px;
    }

    @include media(cs, 0, 1200px) {
      flex-flow: column;
      align-items: center;
      justify-content: center;
      img {
        position: relative;
        bottom: 10px;
      }
      span {
        padding: 0;
      }
    }
  }

  .top-positioner {
    cursor: pointer;
    position: fixed;
    bottom: 88px;
    right: 62px;
    z-index: 9999;
  }


</style>
