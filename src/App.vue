<template>
  <div id="app" class="main-container">
    <app-header></app-header>
    <app-h-nav></app-h-nav>
    <router-view></router-view>
    <app-footer></app-footer>
  </div>
</template>

<style>
.main-container {
  display: block;
  overflow: hidden;
  width: 1200px;
}
</style>
<script>
import AppHeader from "@/components/AppHeader";
import AppHNav from "@/components/AppHNav";
import AppFooter from "@/components/AppFooter";
export default {
  name: "App",
  components: { AppHeader, AppHNav, AppFooter },
};
</script>
