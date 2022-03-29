<!-- Dentro del template solo puede haber un elemento -->
<template>
  <div id="app">
    <home-vue></home-vue>
  </div>
</template>

<script>
import HomeVue from "./components/HomeVue.vue";

export default {
  name: "App",
  components: {
    HomeVue,
  },
};
</script>

<style></style>
