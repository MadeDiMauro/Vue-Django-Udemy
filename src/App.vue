<!-- Dentro del template solo puede haber un elemento -->
<template>
  <div id="app">
    <home-vue v-if="false"></home-vue>
    <pixabay></pixabay>
  </div>
</template>

<script>
import HomeVue from "./components/HomeVue.vue";
import Pixabay from "./components/pixabay/Component-Pixabay.vue";

export default {
  name: "App",
  components: {
    HomeVue,
    Pixabay,
  },
};
</script>

<style></style>
