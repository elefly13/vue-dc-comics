<template>
  <div id="app">
  
    <Header/>
    <Main/>
    <MainIcon/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import MainIcon from './components/MainIcon.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    MainIcon,
    Footer
  }
}
</script>

<style lang="scss">
// @import "../assets/style/generals";
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
  width: 100vw;
  background-color: black;
  font-family: 'Roboto', sans-serif;

}


// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
</style>
