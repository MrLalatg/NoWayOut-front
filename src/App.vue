<template>
  <div id="app">
    <MainPage />
  </div>
</template>

<script>
  import MainPage from "@/components/MainPage";
  export default {
    components: {
      MainPage
    }
  }
</script>

<style>
  body {
    background-image: url("~@/assets/mainbg.jpg");
    background-position: center center;
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-size: cover;
    background-color: #464646;
  }
  @font-face {
    font-family: "Stalker";
    src: local("Stalker"),
    url("~@/fonts/stalker.ttf") format("truetype");
  }
  MainPage{
    height: 100%;
    width: 100%;
  }
</style>
