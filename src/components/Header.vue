<template>
<div class="container">
  <header>
        <a href="/">
                <img src="../assets/img/dc-logo.png" alt="">
            </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index" :class="{ active: link.current }">
                    <a :href="link.url" :class="{ active: link.current }" >{{ link.text }}</a>
                </li>
            </ul>
        </nav>        
  </header>
</div>
</template>

<script>
export default {
    name: "Header",
    props: [ "links" ]
}
</script>

<style lang="scss" scoped>
    @import "../style/variables";
    header{
        line-height: 80px;
        display:flex;
        justify-content: space-between;
        align-items: center;
    }
    img{    
        padding:10px 0px;
        height: 80px;
        vertical-align: middle; 
    }
    ul {
        display: flex;
        justify-content: center;
        list-style: none;
        li {
            height:100%;
            a {
                padding: 15px;
                color: rgba($bgColor,0.8);
                font-weight: 700;
                font-size: 14px;
                text-transform: uppercase;
                text-decoration: none;
            &.active,
            &:hover {
                color: $brandColor;
                }
            }
            &.active{
                border-bottom:4px solid $brandColor;
            }
           
        }
    }
</style>