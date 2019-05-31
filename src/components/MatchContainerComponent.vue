<template>
  <div class="match-container">
    <div class="football">
      <img src="../assets/imgs/Color_Fill_2_copy_3.png">
      <img class="gateWidget" src="../assets/imgs/SkyHD_Pixel-Destruction_Goalkeeper_copy.png">
      <div class="regjister flex-column">
        <p class="title-regjister">
          <span class="first">b365SPORT</span> is simply dummy text of the printing and typesetting <span class="second">industry</span>
        </p>
        <button class="btn-regjister">REGISTRATI ORA!</button>
      </div>
    </div>
    <div class="poker">

    </div>
  </div>
</template>

<script>
  export default {
    name: "MatchContainerComponent"
  }
</script>

<style scoped lang="scss">
  @import "../assets/scss/const";
  @import "../assets/scss/class";

  .match-container {
    width: 1064px;
    height: 559px;
    box-shadow: 0 0 13px #000000;
    border: 3px solid #000000;
    background-color: rgba(44 ,44 , 44 , 0.5);
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    position: absolute;
    margin: auto;
    display: flex;
    .football {
      position: relative;
      .gateWidget {
        position: absolute;
        right: 0;
        bottom: 0;
      }
      .regjister {
        width: 366px;
        .title-regjister {
          color: #ff6000;
          font-family: $font-rajdhani;
          font-size: 21px;
          font-weight: 400;
          line-height: 18.88px;
          text-transform: uppercase;
          .first {
            color: #b4d8f7;
            font-family: $font-rajdhani-bold;
            font-weight: 700;
          }
          .second {
            font-family: $font-rajdhani-regular;
            color: #b4d8f7;
            font-weight: 400;
          }
        }
        .btn-regjister {
          width: 162px;
          height: 36px;
          box-shadow: inset 0 0 10px #000000;
          border-radius: 17px;
          background-color: #f26222;
          color: #ffffff;
          font-family:$font-rajdhani;
          font-size: 18px;
          font-weight: 500;
          line-height: 16px;
          text-transform: uppercase;
        }
      }
    }
    .poker {
      width: 344px;
      height: 559px;
      background-color: #414141;
      opacity: 0.5;
    }
  }



</style>
