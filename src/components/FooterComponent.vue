<template>
  <div>
    <quick-links-component />
  <div class="footer-container w-100">
    <img src="../assets/imgs/Vector_Smart_Object.png">
    <span class="footer-text">© 2001-2017 bet365. All rights reserved.</span>
  </div>
  </div>

</template>

<script>
  import QuickLinksComponent from "./QuickLinksComponent";
  export default {
    name: "FooterComponent",
    components: {QuickLinksComponent}
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
   @include media(cs, 0 , 1200px) {
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


</style>
