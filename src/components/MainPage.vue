<template>
    <div id="main">
        <Header id="header" />
        <Center id="center"/>
        <Footer id="footer" />
    </div>
</template>

<script>
    import Header from "./Header";
    import Center from "./Center";
    import Footer from "./Footer";
    export default {
        name: "MainPage",
        components: {
          Center,
          Header,
          Footer
        }
    }
</script>

<style scoped>
    #main {
        height: 100%;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }
</style>