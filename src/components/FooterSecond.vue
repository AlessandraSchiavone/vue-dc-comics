<template>
  <footer>
      <div class="container">
        <div class="left">
             Sign-up now!
        </div>
        <div class="right">
             Follow us
             <img src="../assets/img/footer-facebook.png" alt="">
             <img src="../assets/img/footer-twitter.png" alt="">
             <img src="../assets/img/footer-youtube.png" alt="">
             <img src="../assets/img/footer-pinterest.png" alt="">
             <img src="../assets/img/footer-periscope.png" alt="">    
        </div>
      </div> 
  </footer>
</template>

<script>
export default {
  name: "FooterSecond"
}
</script>

<style lang="scss" scoped>
 @import "../style/variables";
    footer {
        padding:5px 0px;
        height:110px;
        background-color: rgba($bgColor,0.9);
    }
    .container{
        height:100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .left{
        border:1px solid $brandColor;
        cursor: pointer;
        padding:10px 20px;
        font-size:20px;
        text-transform: uppercase;
        color:white;
        font-weight: 700;
    }
    .right{
        color:$brandColor;
        text-transform: uppercase;
        font-size:20px;
        font-weight: 700;
        img{
            cursor: pointer;
            vertical-align: middle;
            padding:5px 10px;
        }
    }
</style>