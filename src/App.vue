<template>
  <NavBar :logo="logo_src" :alt="app_name" />
  <router-view />
  <Footer />
</template>

<script>
import NavBar from "./components/NavBar";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    NavBar,
    Footer,
  },
  data() {
    return {
      logo_src: "/img/logo.png",
      app_name: "/img/burger.jpg"
    }
  }
};
</script>

<style>
 * {
  font-family: Arial, Helvetica, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
 }

 .main_container {
  margin: 50px;
  min-height: 250px;
}

h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>