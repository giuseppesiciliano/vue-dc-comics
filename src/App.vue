<template>
  <div id="app">
    <Header />
  
    <main>
      <Jumbotron />
      <MagazinesList />
    </main>

    <PreFooter />

    <Footer />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import MagazinesList from "./components/MagazinesList.vue";
import PreFooter from "./components/PreFooter.vue";
import Footer from "./components/Footer.vue";



export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    MagazinesList,
    PreFooter,
    Footer
  },
};
</script>

<style lang="scss">
@import './style/generals.scss';
@import './style/common.scss';

</style>
