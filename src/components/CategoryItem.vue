<template>
  <div class="category-item-category">
    <div class="category-image">
      <a :href="href"><img :src="image" :alt="imageAlt" /></a>
    </div>
    <div class="category-info">
      <a :href="href">{{ genre }}: {{ title }}</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "category-item",
  props: {
    image: {
      type: String,
      required: true,
    },
    imageAlt: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    genre: {
      type: String,
      required: true,
    },
    href: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped></style>
