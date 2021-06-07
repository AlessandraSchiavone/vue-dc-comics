<template>
    <footer>
      <div class="container">
          <div class="cols">
            <div>
            <h3>DC COMICS</h3>
            <nav>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV </a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">News</a></li>
                </ul>
            </nav>
        </div>
        <div>
            <h3>SHOP</h3>
            <nav>
                <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
            </nav>
        </div>   
        <div>
            <h3>DC</h3>
            <nav>
                <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy Police</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Adverstising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshop</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>

                </ul>
            </nav>
        </div>
        <div>
            <h3>Sites</h3>
            <nav>
                <ul>
                    <li><a href="#">DC </a></li>
                    <li><a href="#">MD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </nav>
        </div>
        
          </div>
          <div class="big-logo">
              <img src="../assets/img/dc-logo-bg.png" alt="">
          </div>
      </div>
    </footer>
</template>

<script>
export default {
    name: "FooterFirst"
}
</script>

<style lang="scss" scoped>
    @import "../style/variables";
    footer {
        background: url('../assets/img/footer-bg.jpg');
        background-size: 100% auto;
    }
    .container{
        display: flex;
        height:380px;
    }
    .cols {
        padding:30px 0px;
        width:50%;
        display: flex; 
        flex-direction: column;
        flex-wrap: wrap;   
    }
    .big-logo{
        width:50%;
        overflow: hidden;
        img{
            width:100%;   
            transform: translateY(-15%);
        }
    }

    .cols > div {
        padding:10px 0px;
        width: calc(100% / 3);
    }
    ul {
        list-style: none;
    }
    li a {
        display: block;
        padding: 2px 0;
        text-decoration: none;
        color: #797979;
        font-size: 14px;
    }
    li a:hover {
        text-decoration: underline;
    }
    h3 {
        margin-bottom: 10px;
        text-transform: uppercase;
        color: white;
        font-size: 20px;
    }
</style>