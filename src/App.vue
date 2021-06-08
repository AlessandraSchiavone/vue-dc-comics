<template>
  <div id="app">
     <!-- testata della pagina -->
    <Header :links="menu" />
    <!-- /testata della pagina -->

    <!-- corpo della pagina -->
    <main>
      <Jumbotron />
      <Series/>
      <Buy />
    </main>
    <!-- /corpo della pagina -->

    <!-- chiusura della pagina -->
    <FooterFirst /> 
    <FooterSecond />

    <!-- /chiusura della pagina -->
  </div>
</template>

<script>
import Header from './components/Header';
import Jumbotron from './components/Jumbotron';
import FooterFirst from './components/FooterFirst';
import FooterSecond from './components/FooterSecond';
import Buy from './components/Buy';
import Series from './components/Series';

export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Series,
    Buy,
    FooterFirst,
    FooterSecond 
  },
  data: function() {
    return {
      menu: [
              {
                    text: "Characters",
                    url: "#characters",
                    current: false
              },
              {
                    text: "Comics",
                    url: "#comics",
                    current: true
              },
              {
                    text: "Movies",
                    url: "#movies",
                    current: false
              },
              {
                    text: "Tv",
                    url: "#tv",
                    current: false
              },
              {
                    text: "Games",
                    url: "#games",
                    current: false
              },
              {
                    text: "Collectibles",
                    url: "#collectibles",
                    current: false
              },
              {
                    text: "Videos",
                    url: "#videos",
                    current: false
              },
              {
                    text: "Fans",
                    url: "#fans",
                    current: false
              },
              {
                    text: "News",
                    url: "#news",
                    current: false
              },
              {
                    text: "Shop",
                    url: "#shop",
                    current: false
              }
          ]
    }
  }
}
</script>

<style lang="scss">
@import "./style/general.scss";
</style>
