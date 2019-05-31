<template>
    <div class="match-container">
      <div class="football">
        <img src="../assets/imgs/Color_Fill_2_copy_3.png">
        <img class="gateWidget" src="../assets/imgs/SkyHD_Pixel-Destruction_Goalkeeper_copy.png">
        <div class="register flex-column">
          <p class="title-register">
            <span class="sport-365-text">b365SPORT</span> is simply dummy text of the printing and typesetting <span class="industry-text">industry</span>
          </p>
          <button class="btn-register">REGISTRATI ORA!</button>
        </div>
      </div>
      <div class="poker">
        <img class="pd-8 pd-btm-0" src="../assets/imgs/Color_Fill_2_copy_4.png">
        <img class="pd-8 pd-btm-0" src="../assets/imgs/Color_Fill_2_copy_5.png">
        <div class="poker-descripsion">VIRTUAL GAMES <span>GIOCA ORA</span></div>
        <img class="pd-8" src="../assets/imgs/Color_Fill_2_copy_7.png">
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
    box-shadow: 0 0 13px #000000;
    border: 3px solid #000000;
    background-color: rgba(44 ,44 , 44 , 0.5);
    margin: auto;
    left: 0;
    right: 0;
    position: relative;
    display: flex;
    .football {
      position: relative;
      .gateWidget {
        position: absolute;
        right: 0;
        bottom: 0;
        width: 366px;
        height: 259px;
      }
      .register {
        width: 405px;
        margin: 17px 0 35px 25px;
        .title-register {
          color: #ff6000;
          font-family: $font-rajdhani;
          font-size: 21px;
          font-weight: 400;
          line-height: 18.88px;
          text-transform: uppercase;
          .sport-365-text {
            color: #b4d8f7;
            font-family: $font-rajdhani-bold;
            font-weight: 700;
          }
          .industry-text {
            font-family: $font-rajdhani-regular;
            color: #b4d8f7;
            font-weight: 400;
          }
        }
        .btn-register {
          white-space: nowrap;
          height: 36px;
          width: min-content;
          padding: 6px 21px;
          box-shadow: inset 0 0 10px #000000;
          border: none;
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
      background-color: rgba(44 ,44 , 44 , 0.5);
      display: flex;
      flex-flow: column;
      img {
        /*padding: 8px;*/
      }
      .poker-descripsion {
        display: flex;
        height: 43px;
        align-items: center;
        background-color: #282828;
        margin: 0 8px;
        font-size: 0.8em;
        justify-content: space-between;
        padding-left: 15px;
        color: #ffffff;
        font-family: $font-rajdhani;
        font-weight: 500;
        line-height: 16px;
        text-transform: uppercase;
        span {
          background-image: url("../assets/imgs/Layer_1.png");
          /*background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHEAAAArCAYAAABPa2dBAAAABGdBT…sAQiNAWFaeb8s8jOvNCtwA8RsB+sD8fkdSWUl3JOTDNNV/r72N5ZbLfIsAAAAASUVORK5CYII=);*/
          background-repeat: no-repeat;
          height: 100%;
          display: flex;
          align-items: center;
          justify-content: center;
          background-size: cover;
          width: 130px;
          padding-left: 10px;
          color: #ff6000;
        }
      }
    }
  }



</style>
