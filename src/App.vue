<script>
import Navbar from "./components/partials/Navbar.vue";
import Footer from "./components/partials/Footer.vue";
import Header from "./components/app/Header.vue";

export default {
  components: {
    Navbar,
    Footer,
    Header,
  },
  data() {
    return {
      isDarkMode: false,
    };
  },
};
</script>

<template>
  <div id="app">
    <Navbar />
    <Header />
    <router-view />
    <Footer />
  </div>
</template>
