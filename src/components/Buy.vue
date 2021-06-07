<template>
    <section>
        <div class="container">
          <div>
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">
              <span>Digital Comics</span>
          </div>
          <div>
              <img src="../assets/img/buy-comics-merchandise.png" alt="">
              <span>DC Merchandise</span>
          </div>
          <div>
              <img src="../assets/img/buy-comics-subscriptions.png" alt="">
              <span>Subscription</span>
          </div>
          <div>
              <img src="../assets/img/buy-comics-shop-locator.png" alt="">
              <span>Comic Shop Locator</span>
          </div>
          <div>
              <img src="../assets/img/buy-dc-power-visa.svg" alt="">
              <span>Dc power visa</span>
          </div>
        </div>
  </section> 
</template>

<script>
export default {
    name: "Buy",
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