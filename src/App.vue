<template>
  <div id="app">
    <Header />
  
    <main>
      <MagazinesList />
    </main>

    <PreFooter />

    <Footer />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import PreFooter from "./components/PreFooter.vue";
import Footer from "./components/Footer.vue";
import MagazinesList from "./components/MagazinesList.vue";



export default {
  name: "App",
  components: {
    Header,
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
