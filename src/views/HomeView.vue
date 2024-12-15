<template>
  <Banner />
  <div class="main_container">
    <h1>Monte o seu burguer:</h1>
    <BurgerForm />
  </div>
</template>

<script>
import BurgerForm from "@/components/BurgerForm.vue";
import Banner from "../components/Banner.vue";

export default {
  name: "HomeView",
  components: {
    Banner,
    BurgerForm,
  },
};
</script>
