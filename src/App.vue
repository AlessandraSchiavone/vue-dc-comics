<template>
  <div id="app">
     <!-- testata della pagina -->
    <Header />
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
    FooterFirst,
    FooterSecond,
    Buy,
    Series
  }
}
</script>

<style lang="scss">
@import "./style/general.scss";
</style>
