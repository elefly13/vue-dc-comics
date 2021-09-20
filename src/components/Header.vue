<template>
  <header>
    <div class="box_header">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="logo-dc">
      </div>
      <nav>
        <ul>
          <li v-for="(link,index) in links" :key="index">
            <a href="#" :class="(link.current) ? 'active' : null">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
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
          current: true,
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
      ]
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
    height: 130px;
    margin-top: 50px;
    background-color: white;

        .box-header {
            width: 70%;
            height: 130px;

            ul {
            list-style: none;
            @include center();

                li a {
                display: inline-block;
                padding: 10px;
                text-decoration: none;
                font-weight: 600;
                color: $secondary;

                    &:hover,
                    &.active {
                        color: $primary;
                    }
                }    
            }
        }    
    }

</style>