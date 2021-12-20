<template>
  <div id="app">
    <Header />
  
    <main>
      <section class="container">
        <h3>Content goes here</h3>
      </section>
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
@import './style/generals.scss';
@import './style/common.scss';

main {
  background-color: black;
  color: white;
  height: 100px;
}
</style>
