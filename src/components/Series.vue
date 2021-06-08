<template>
    <section>
        <div class="container">
            <span class="btn btn-current">
                Current Series
            </span>
            <div class="series-cont">
                <Serie 
                    v-for="(serie, index) in series"
                    :key="index"
                    :single-product="serie"
                /> 
            <span class="btn btn-load">
                Load More
            </span> 
            </div>
            
        </div>
    </section>
</template>

<script>
import Serie from './Serie';
import cardser from '../data/cardser';
export default {
    name:"Series",
    components: {
       Serie
    },
    data: function() {
        return {
            series: cardser
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables";
section{
    position:relative;
    background-color: $bgColor;
}
.series-cont{
    padding:60px 0px;
    position:relative;
    display: flex;
    flex-wrap: wrap;
}
.btn{
    color:white;
    font-weight: 700;
    text-transform: uppercase;
    background-color: $brandColor;
}
.btn-current{
    position:absolute;
    top:-28px;
    font-size: 28px;
    padding:10px 20px; 
}
.btn-load{
    cursor: pointer;
    position:absolute;
    right:50%;
    bottom:2%;
    transform: translateX(50%);
    font-size: 13px;
    padding:10px 50px;
}

</style>