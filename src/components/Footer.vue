<template>
  <div id="footer">
    <div id="imgLinks" style="width: 33%; padding-left: 50px">
      <a href="https://discord.gg/Z8sDr9fYCT" target="_blank">
        <img class="hov" src="../assets/discord_negate.png" alt="" style="margin-right: 10px">
      </a>
      <a href="https://vk.com/nowayoutstalkerrp" target="_blank">
        <img class="hov" src="../assets/vk_negate.png" alt="">
      </a>
    </div>
    <div style="width: 33%; display: flex; justify-content: center">
      <img src="../assets/dayzlogo.png" alt="">
    </div>
    <div style="width: 33%; display: flex; justify-content: flex-end; padding-right: 50px">
      <h2>
        Сталкер онлайн на базе DayZ
      </h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
}
</script>

<style scoped>
  #footer {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
  }
  h2 {
    font-family: gotham, Serif;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    line-height: 19px;
    color: white;
  }
  .hov:hover {
    -webkit-transform: scale(1.2);
    -ms-transform: scale(1.2);
    transform: scale(1.2);
  }
</style>