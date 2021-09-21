<template>
  <div class="box-footer">
    <div class="container">
      <div class="box-img">
      <img src="@/assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    
    
    
    
  </div>

</template>

<script>
export default {
  name: 'Footer',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/vars.scss";

.box-footer {
  width: 100vw;
  height: 400px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: 100%;

    .container {
      width: 70%;
      height: 100%;
      margin: 0 auto;
        .box-img {
          
          width: 600px;
          height: 400px;
          float: right;
            img {
              width: 100%;
              height: 100%;
              object-fit: none;
            }
        }
    }
}


</style>