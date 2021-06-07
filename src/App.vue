<template>
  <div id="app">
     <!-- testata della pagina -->
    <Header />
    <!-- /testata della pagina -->

    <!-- corpo della pagina -->
    <main>
      <Contents />
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
import Contents from './components/Contents';
import FooterFirst from './components/FooterFirst';
import FooterSecond from './components/FooterSecond';
import Buy from './components/Buy';

export default {
  name: 'App',
  components: {
    Header,
    Contents,
    FooterFirst,
    FooterSecond,
    Buy
  }
}
</script>

<style lang="scss">
@import "./style/general.scss";
</style>
