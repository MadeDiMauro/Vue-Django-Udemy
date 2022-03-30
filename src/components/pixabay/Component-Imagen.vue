<template>
  <div><b-img thumbnail fluid :id="img.id" :src="img.previewURL"></b-img></div>
</template>

<script>
export default {
  name: "Component-Imagen",
  props: ["img"],
};
</script>
<style scoped></style>
