<template>
<div class="container-foot">
    <div class="box-foot">
        <button class="btn">SIGN UP NOW!</button>
        
        <div class="box-social" >
            <h2>FOLLOW US</h2>
            <div class="icona" v-for="(ico,index) in social" :key="index">
                <img :src="require(`../${ico.icona}`)" alt="">
            </div>
        </div>

    </div>

</div>
  
</template>

<script>
export default {
    name: 'FootFoot',
        data() {
            return {
                social: [
                    {
                    icona: "assets/img/footer-facebook.png",
                    url: "#"  
                    },
                    {
                    icona: "assets/img/footer-periscope.png",
                    url: "#"  
                    },
                    {
                    icona: "assets/img/footer-pinterest.png",
                    url: "#"  
                    },
                    {
                    icona: "assets/img/footer-twitter.png", 
                    url: "#"
                    },
                    {
                    icona: "assets/img/footer-youtube.png", 
                    url: "#" 
                    }
                ]
            }
        }    
}
</script>

<style scoped lang="scss">
@import "../assets/style/vars.scss";

.container-foot {
    width: 100vw;
    height: 170px;
    background-color: rgb(47, 47, 47);
    .box-foot {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 70%;
        height: 170px;
        margin: 0 auto;
        
            .btn {
                width: 170px;
                height: 60px;
                border: 2px solid $primary;
                background-color:rgb(47, 47, 47);
                color: $secondary;
                font-size: 17px;
            }
            
            .box-social {
                display: flex;
                align-items: center;
                align-content: flex-end; 
                    h2 {
                
                    color: $primary;
                    margin-right: 30px;
                    }   
                    .icona {
                    width: 50px;
                    height: 50px;
                    margin-left: 20px;
                        img {
                            width: 100%;
                        }
                    
                    }
            }
            
    }
}

</style>