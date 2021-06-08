<template>
    <section>
        <div class="container">
          <div v-for="(buy, index) in buys" :key="index">
              <img :src="buy.src" :alt="buy.text">
              <span>{{ buy.text }}</span>
          </div>
        </div>
  </section> 
</template>

<script>
export default {
    name: "Buy",
    data: function(){
        return {
            buys:[
                {
                    src:require("../assets/img/buy-comics-digital-comics.png"),
                    text:"Digital Comics"
                },
                {
                    src:require("../assets/img/buy-comics-merchandise.png"),
                    text:"DC Merchandise"
                },
                {
                    src:require("../assets/img/buy-comics-subscriptions.png"),
                    text:"Subscription"
                },
                {
                    src:require("../assets/img/buy-comics-shop-locator.png"),
                    text:"Comic Shop Locator"
                },
                {
                    src:require("../assets/img/buy-dc-power-visa.svg"),
                    text:"Dc power visa"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../style/variables";
    section{
        background-color:$brandColor;
        height: 150px;
    }
    .container{
        height: 100%;
        display: flex;
        justify-content:space-around;
        align-items: center;
    }
    div{
        display: flex;
        justify-content: center;
        align-items: center;
        img{
            padding:5px;
            height:55px;
        }
        span{
            font-size: 15px;
            padding:0px 5px;
            color:white;
            text-transform: uppercase;
        }
    }
</style>