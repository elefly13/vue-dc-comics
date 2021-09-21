<template>
  <div class="box-main" >
    
    <div class="nav-main">
      <div class="item-nav"  v-for="(ico,index) in icone" :key="index">
        <div class="box-img">
          <img :src="require(`../${ico.icon}`)" alt="ico.name">     
        </div>
        <div class="text-nav">{{ ico.name }}</div>
      </div>

  
       
    </div>
   
  </div>
</template>

<script>
export default {
  name: 'MainIcon',
  
  data() {
    return {
      icone: [
        {
          name: "DIGITAL COMICS",
          icon: "assets/img/buy-comics-digital-comics.png",
          url: "#"
        },
        {
          name: "DC MERCHANDISE",
          icon: "assets/img/buy-comics-merchandise.png",
          url: "#"
        },
        {
          name: "SUBSCRIPTION",
          icon: "assets/img/buy-comics-subscriptions.png",
          url: "#"
        },
        {
          name: "COMIC SHOP LOCATOR",
          icon: "assets/img/buy-comics-shop-locator.png",
          url: "#"
        },
        {
          name: "DC POWER VISA",
          icon: "assets/img/buy-dc-power-visa.svg",
          url: "#"
        }
      ]
    }      
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/vars.scss";

.box-main {
  width: 100%;
  height: 200px;
  background-color: $primary;
  
  
  .nav-main {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 70%;
    height: 200px;
    margin: 0 auto;

    .item-nav {
      display: flex;
      align-items: center;
      width: 20%;
      height: 100px;
        .box-img {
          width: 80px;
            img {
              display: cover;
              width: 70%;
            }
        }
        .text-nav {
          color: white;
          padding-left: 20px;
        }
     
    }
  }

  
}


</style>