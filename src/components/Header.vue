<template>
  <div id="header">
    <div id="headerLogo">
        <img src="../assets/headerlogo.png" alt="">
      <div id="spacer1"></div>
    </div>
    <div id="links">
      <a href="https://discord.gg/Z8sDr9fYCT" target="_blank" style="margin-right: 30px">Дискорд</a>
      <a href="https://steamcommunity.com/sharedfiles/filedetails/?id=2649514486" target="_blank" style="margin-right: 30px">Steam</a>
      <a href="https://vk.com/nowayoutstalkerrp" target="_blank">Вконтакте</a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Header"
  }
</script>

<style scoped>
  #header {
    display: flex;
    align-items: center;
  }


  #spacer1{
    flex: 1;
  }

  #headerLogo {
    flex: 2;
    display: flex;
    justify-content: flex-start;
    align-items: center;
    padding-left: 50px;
  }

  p {
    font-family: Stalker, serif;
    font-style: normal;
    font-weight: 400;
    font-size: 60px;
    color: white;
    margin: 0;
    padding: 0;
  }

  #links {
    flex: 1;
    font-family: gotham, serif;
    font-style: normal;
    font-weight: normal;
    font-size: 20px;
    display: flex;
    justify-content: flex-end;
    padding-right: 50px;
    gap: 10px;
  }

  a {
    color: white;
  }

  a:hover {
    color: #666666;
  }
</style>