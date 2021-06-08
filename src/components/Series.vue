<template>
    <section>
        <div class="container">
            <span class="btn-current">
                Current Series
            </span>
            <span class="btn-load">
                Load More
            </span>
        </div>
    </section>
</template>

<script>
export default {
    name:"Series"
}
</script>

<style lang="scss" scoped>
@import "../style/variables";
section{
    position:relative;
    height:600px;
    background-color: #1C1C1C;
}
.btn-current{
    position:absolute;
    top:-28px;
    font-size: 28px;
    color:white;
    padding:10px 20px;
    font-weight: 700;
    text-transform: uppercase;
    background-color: $brandColor;
}
.btn-load{
    position:absolute;
    right:50%;
    bottom:4%;
    font-weight: 700;
    text-transform: uppercase;
    padding:10px 50px;
    color:white;
    background-color: $brandColor;
}

</style>