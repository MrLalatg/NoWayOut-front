<template>
  <div id="center">
    <div id="content">
      <div id="descr">
        <p id="big">NO WAY OUT</p>
        <h2>Тебя ждет:</h2>
        <ul>
          <li>живое общение с игроками</li>
          <li>эмоции и выживание в зоне</li>
          <li>красивая современная графика</li>
          <li>ситуации которые изменят всю зону</li>
        </ul>
        <div id="btn">
          <a href="https://vk.com/nowayoutstalkerrp?w=wall-40278937_124" target="_blank">
            <div style="display:flex; justify-content: center; align-items: center; flex: 1" @mouseenter="infoButtonHover" @mouseleave="infoButtonHover">
              <h2 id="btntext">Подробнее</h2>
              <img :src="bInfoPath" alt="">
            </div>
          </a>
          <div style="display: flex; align-items: center; flex: 1; margin-left: 47px">
            <a href="https://vk.com/nowayoutstalkerrp?w=wall-40278937_124" target="_blank"><h2><u>Как начать играть</u></h2></a>
          </div>
        </div>
      </div>
    </div>
    <div id="spacer"></div>
  </div>
</template>

<script>
  export default {
    name: "Center",
    data: function () {
      return {
        moreInfoState: false,
        bInfoPath: require("../assets/moreInfoBtn.png")
      }
    },
    methods: {
      infoButtonHover(){
        if(this.moreInfoState){
          this.bInfoPath = require("../assets/moreInfoBtn.png");
          this.moreInfoState = false;
        } else {
          this.bInfoPath = require("../assets/infoBtnHover.png");
          this.moreInfoState = true;
        }
      }
    }
  }
</script>

<style scoped>
  a:link {
    text-decoration: inherit;
    color: inherit;
    cursor: auto;
  }

  a:visited {
    text-decoration: inherit;
    color: inherit;
    cursor: auto;
  }
  #center {
    display: flex;
    justify-content: space-around;
  }

  #content {
    flex: 1;
    display: flex;
    justify-content: flex-end;
  }

  #spacer {
    flex: 1;
  }

  #big {
    font-family: Stalker, serif;
    font-style: normal;
    font-weight: normal;
    font-size: 130px;
    line-height: 188px;
    letter-spacing: 0.13em;
    color: #FFFFFF;
    text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    margin-top: 0;
  }

  h2 {
    font-family: gotham, Serif;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 19px;
    color: white;
  }

  p {
    margin-bottom: 0;
  }

  li {
    font-family: gotham, Serif;
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    color: white;
    margin: 5px;
  }

  #btntext {
    position: absolute;
  }

  #btn {
    display: flex;
    margin-top: 50px;
  }

  u:hover{
    color: #666666;
  }
</style>