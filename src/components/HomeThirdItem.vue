<template>
  <div class="page-third">
    <div class="page-card page-container">
      <div class="front-page-image-container">
        <img :src="image" :alt="imageAlt" />
      </div>
      <div class="front-page-third-text">
        <a :href="href">{{ text }}</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home-third-item",
  props: {
    image: {
      type: String,
      required: true,
    },
    imageAlt: {
      type: String,
      required: true,
    },
    text: {
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

<style scoped>
.page-third .page-card {
  padding-left: 0px;
  padding-right: 0px;
}

.front-page-image-container {
  padding: 0;
  margin: 0;
}

.front-page-image-container img {
  width: 100%;
}

.front-page-third-text {
  text-align: center;
  font-size: larger;
  padding: 15px;
}

.front-page-third-text a {
  text-decoration: none;
  color: black;
}

.front-page-third-text a:hover {
  text-decoration: underline;
  color: var(--Grey);
}
</style>
