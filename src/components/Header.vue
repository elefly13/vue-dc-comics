<template>
  <header>
    <div class="box-header">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="logo-dc">
      </div>
      <div class="nav">
        <ul>
          <li v-for="(link,index) in links" :key="index">
            <a href="#" :class="(link.current) ? 'active' : null">{{ link.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',

  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          text: "COMICS",
          url: "#",
          current: false,
        },
        {
          text: "MOVIES",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "GAMES",
          url: "#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false,
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false,
        },
        {
          text: "FANS",
          url: "#",
          current: false,
        },
        {
          text: "NEWS",
          url: "#",
          current: false,
        },{
          text: "SHOP",
          url: "#",
          current: false,
        }
      ],
    }
    
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/vars.scss";
    @import "../assets/style/mixins.scss";

    header {
     width: 100%;
     height: 170px;
     background-color: $secondary;

        .box-header {
            width: 70%;
            height: 170px;
            margin: 0 auto;
             @include center();

            .logo {
                width: 100px;
                height: 100px;

                img {
                    width: 100px;
                }
            }

            ul {
              
            display: flex;
            justify-content: flex-end;
            list-style: none;
           
                li {

                display: inline-block;

                    a {
                    display: inline-block;
                    line-height: 145px;
                    padding: 10px;
                    text-decoration: none;
                    font-weight: 600;
                    color: black;
                    

                        &:hover,
                        &.active {
                            color: $primary;
                            border-bottom: 5px solid $primary;
                        }
                    }    
                }

                
            }
        }    
    }

</style>