<template>
  <div id="v-nav" class="clearfix">
    <div class="v-nav-content">
      <div class="menu-title">
        <span class="text">Favorites</span>
        <span class="chevron"
          ><font-awesome-icon icon="fa-solid fa-chevron-down"
        /></span>
      </div>
      <div class="menu-item">
        <i class="fa-regular fa-square-check"></i> Best Sellers
      </div>
      <div class="menu-item">
        <i class="fa-regular fa-square"></i> New Releases
      </div>
      <div class="menu-item"><i class="fa-regular fa-square"></i> In Stock</div>

      <div class="menu-title">
        <span class="text">Condition</span>
        <span class="chevron"
          ><font-awesome-icon icon="fa-solid fa-chevron-down"
        /></span>
      </div>
      <div class="menu-item">
        <i class="fa-regular fa-square-check"></i> All
      </div>
      <div class="menu-item"><i class="fa-regular fa-square"></i> New</div>
      <div class="menu-item"><i class="fa-regular fa-square"></i> Used</div>

      <div class="menu-title">
        <span class="text">Format</span>
        <span class="chevron"
          ><font-awesome-icon icon="fa-solid fa-chevron-down"
        /></span>
      </div>
      <div class="menu-item">
        <i class="fa-regular fa-square-check"></i> All
      </div>
      <div class="menu-item">
        <i class="fa-regular fa-square"></i> Hardcover
      </div>
      <div class="menu-item">
        <i class="fa-regular fa-square"></i> Paperback
      </div>
      <div class="menu-item"><i class="fa-regular fa-square"></i> eBook</div>
      <div class="menu-item"><i class="fa-regular fa-square"></i> Textbook</div>

      <div class="menu-title">
        <span class="text">More</span>
        <span class="chevron"
          ><font-awesome-icon icon="fa-solid fa-chevron-right"
        /></span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "category-v-nav",
};
</script>
<style scoped>
#v-nav {
  padding-left: 15px;
  padding-bottom: 15px;
}

.v-nav-content {
  max-width: 100%;
  min-width: 175px;
  border: 1px var(--BorderShade) solid;
}

#v-nav .menu-title {
  background-color: var(--PrimaryColor);
  padding: 10px;
  color: #fff;
}

#v-nav .menu-title .text {
}

#v-nav .menu-title .chevron {
  float: right;
}

#v-nav .menu-item {
  padding: 5px;
  padding-left: 15px;
}
</style>
