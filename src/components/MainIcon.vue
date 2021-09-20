<template>
  <div class="box-main" >
    
    <div class="nav-main">
      <div class="item-nav">

      </div>
    </div>
   
  </div>
</template>

<script>
export default {
  name: 'MainIcon',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/vars.scss";

.box-main {
  width: 100%;
  height: 200px;
  
  
  .nav-main {
    width: 100%;
    height: 200px;
    background-color: $primary;

    .item-nav {
      width: 70%;
      height: 200px;
      margin: 0 auto;
      background-color: $primary;
    }
  }

  
}


</style>