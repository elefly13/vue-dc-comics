<template>
  <div class="box-main" >
    <div class="content">
       <h1>- ->Content goes here  - - </h1>
    </div>
    <div class="nav-main">
      <div class="item-nav">

      </div>

    </div>
   
  </div>
</template>

<script>
export default {
  name: 'Main',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/vars.scss";

.box-main {
  width: 100%;
  height: 370px;
  .content {
    display: flex;
    justify-content: left;
    align-items: center;
    width: 70%;
    height: 170px;
    margin: 0 auto;
    h1 {
      color: white;
      text-align: center;
    }
  }
  .nav-main {
    width: 100%;
    height: 200px;
    background-color: $primary;

    .item-nav {
      width: 70%;
      height: 200px;
      margin: 0 auto;
      background-color: violet;
    }
  }

  
}


</style>