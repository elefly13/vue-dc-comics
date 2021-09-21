<template>
  <div class="box-footer">
    <div class="container">
      <div class="list">
        <ul>
          <h3>DC COMICS</h3>
          <li>Caracters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
        <ul>
          <h3>SHOP</h3>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </div><div class="list">
        <ul>
          <h3>DC</h3>
          <li>Terms of use</li>
          <li>Privacy Policy (News)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>
      </div>
      <div class="list">
        <ul>
          <h3>SITES</h3>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>
      <div class="box-img">
      <img src="@/assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    <FootFoot/>
  
  </div>

</template>

<script>
import FootFoot from '@/components/FootFoot.vue'
export default {
  name: 'Footer',
 components: {
    FootFoot
  },
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
        .list {
          float: left;
          height: 300px;
          padding: 30px 0;
          margin-left: 30px;
            h3 {
            color: $secondary;
            padding: 10px 0;
          }
            li {
            list-style: none;
            color: gray;
            font-size: 15px;
            padding: 5px 0;
          }
        }
        
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