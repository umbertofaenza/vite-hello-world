<script>
export default {
  data() {
    return {
      imagePath: "img/jumbotron.jpg",
    };
  },

  methods: {
    getImagePath(path) {
      return new URL(`../assets/${path}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <img :src="getImagePath(imagePath)" alt="Jumbotron" />
</template>

<style scoped></style>
