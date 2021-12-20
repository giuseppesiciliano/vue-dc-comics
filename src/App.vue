<template>
  <div id="app">
    <Header />
  
    <main>
      <h3>Content goes here</h3>
    </main>

    <PreFooter />
    <Footer />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import PreFooter from "./components/PreFooter.vue";
import Footer from "./components/Footer.vue";


export default {
  name: "App",
  components: {
    Header,
    PreFooter,
    Footer
  },
};
</script>

<style lang="scss">

</style>
