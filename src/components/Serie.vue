<template>
   <div class="card">
       <div class="img-cont">
           <img :src="singleProduct.thumb" :alt="singleProduct.series">
       </div>
       <div class="text">{{singleProduct.series}}</div>
  </div>
</template>

<script>
export default {
    name: "Serie",
    props: ["singleProduct"]
}
</script>
<style lang="scss">
    .card {
        width: calc(100% / 6);
        padding:10px;
        .img-cont{
          height:180px;
          overflow: hidden; 
        }
        .text{
            padding:20px 0px;
            font-size:15px;
            color:white;
            text-transform: uppercase;
        }
    }
</style>