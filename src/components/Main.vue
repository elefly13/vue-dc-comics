<template>
  <div class="box-main" >
    <div class="jumbotron">
      <div class="box-container">
        <div class="current">CURRENT SERIES</div>
      </div>
    </div>
    <MainSeries/>
  </div>
</template>

<script>
import MainSeries from '@/components/MainSeries.vue'
// import Series from 'Series.js'
export default {
  name: 'Main',
  components: {
    MainSeries
  },
  // data() {
  //   return {
  //     series: Series
  //   }
  // }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import "../assets/style/vars.scss";

.box-main {
  width: 100vw;
 
  .jumbotron {
    
    width: 100%;
    height: 450px;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: 100%;
      .box-container {
        position: relative;
        width: 70%;
        height: 450px;
        margin: 0 auto;
          .current {
          position: absolute;
          left: 0;
          bottom: -30px;
          width: 200px;
          height: 70px;
          background-color: $primary;
          color: $secondary;
          text-align: center;
          line-height: 70px;
          font-weight: 900;
          font-size: 20px;

        }
      }
      
  }
}


</style>