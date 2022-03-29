<template>
  <div id="HomeVue">
    <b-container>
      <b-row>
        <b-col>
          <h1>
            Bienvenidos al sistema de facturación
            <small>Hecho por Maddie</small>
          </h1>
          <img
            src="../assets/facturacion-banner.jpg"
            alt=""
            width="100%"
            height="auto"
            rounded="circle"
          />
        </b-col>
      </b-row>
      <b-row>
        <b-col v-for="red in redes" :key="red.red" class="text-center">
          <b-link :href="red.url" target="_blank">
            <b-alert :variant="red.color" show>{{ red.red }}</b-alert>
          </b-link>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "HomeVue",
  data() {
    return {
      redes: [
        {
          red: "facebook",
          url: "https://facebook.com",
          color: "info",
        },
        {
          red: "twitter",
          url: "https://twitter.com",
          color: "warning",
        },
        {
          red: "youtube",
          url: "https://youtube.com",
          color: "danger",
        },
      ],
    };
  },
};
</script>

<style></style>
