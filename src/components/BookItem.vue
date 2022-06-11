<template>
  <div class="category-item-book">
    <div class="category-image">
      <a :href="href"><img :src="image" :alt="imageAlt" /></a>
    </div>
    <div class="category-info">
      <span class="category-info-line"
        ><a :href="href">{{ title }}</a></span
      ><br />
      <span class="category-info-line">by {{ author }}</span
      ><br />
      <span class="category-info-line"
        ><a :href="href"
          >Add to Cart | $21.59
          <font-awesome-icon icon="fa-solid fa-cart-plus" /></a
      ></span>
    </div>
  </div>
</template>

<script>
export default {
  name: "book-item",
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
    author: {
      type: String,
      required: true,
    },
    href: {
      type: String,
      required: true,
    },
    freeRead: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped></style>
