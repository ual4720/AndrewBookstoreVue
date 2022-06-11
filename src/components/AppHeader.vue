<template>
  <!-- #### header Code #### -->
  <header id="header" class="clearfix">
    <div class="logo_container">
      &nbsp;<!--<img class="logo" src="images/logo_transparent_1080x1080.png">-->
    </div>
    <div class="slogan">Explore Your Imagination with Prose</div>
    <app-header-search></app-header-search>
  </header>
  <!-- #### End header Code #### -->
</template>

<script>
import AppHeaderSearch from "@/components/AppHeaderSearch";
export default {
  name: "AppHeader",
  components: { AppHeaderSearch },
  component: {
    AppHeaderSearch,
  },
};
</script>

<style scoped>
header {
  width: 100%;
  background-color: var(--PrimaryColor);
  background-image: url("../assets/images/banner_bg.png");
  background-position: center;
  background-size: cover;
  min-height: 200px;
  padding: 0;
  margin: 0;
}

header div {
  float: left;
}

.logo_container {
  width: 200px;
  height: 200px;
  padding: 0;
  background-image: url("../assets/images/logo_transparent_1080x1080.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: 250px 250px;
}

.slogan {
  text-align: center;
  height: 35px;
  margin-top: 75px;
  padding-left: 0;
  padding-top: 4px;
  color: #fff;
  font-size: 24px; /* Use the auto sizing viewport to make text adjust size */
}

.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>
