<template>
  <!-- #### main Code #### -->
  <main id="main" class="clearfix">
    <section class="content_container">
      <app-page-title :title="page.title" />
      <div class="page-quarter">
        <category-v-nav></category-v-nav>
      </div>
      <div class="page-threequarter">
        <div class="category-line clearfix">
          <div class="category-title">
            <table class="category-table">
              <tr>
                <td class="col-color">&nbsp;</td>
                <td class="col-text">Top Categories</td>
              </tr>
            </table>
          </div>
          <div class="category-content">
            <category-item
              v-for="(item, index) in categories"
              v-bind:key="index"
              :genre="item.genre"
              :title="item.title"
              :href="item.href"
              :imageAlt="item.imageAlt"
              :image="item.image"
            ></category-item>
          </div>
          <div class="category-more">
            <button class="button button-tertiary">More...</button>
          </div>
        </div>
        <div class="page-space">&nbsp;</div>
        <div class="category-line clearfix">
          <div class="category-title">
            <table class="category-table">
              <tr>
                <td class="col-color">&nbsp;</td>
                <td class="col-text">Favorite Books</td>
              </tr>
            </table>
          </div>
          <div class="category-content">
            <book-item
              v-for="(item, index) in books"
              v-bind:key="index"
              :title="item.title"
              :author="item.author"
              :href="item.href"
              :imageAlt="item.imageAlt"
              :image="item.image"
              :free-read="false"
            ></book-item>
          </div>
          <div class="category-more">
            <button class="button button-tertiary">More...</button>
          </div>
        </div>
      </div>
      <div class="page-space">&nbsp;</div>
    </section>
  </main>
  <!-- #### End main Code #### -->
</template>

<script>
// @ is an alias to /src
import AppPageTitle from "@/components/AppPageTitle";
import CategoryVNav from "@/components/CategoryVNav";
import CategoryItem from "@/components/CategoryItem";
import BookItem from "@/components/BookItem";
import "@/assets/css/page-category.css";
import fictionClassics from "../assets/images/categories/classics.png";
import fictionMystery from "../assets/images/categories/mystery.png";
import howToHomediy from "../assets/images/categories/homediy.png";
import bookGaia from "../assets/images/books/gaia_garden.png";
import bookBookcases from "../assets/images/books/bookcases_cabinets.png";
import bookIlluminated from "../assets/images/books/computerscience_illuminated.png";

export default {
  name: "CategoryView",
  components: {
    AppPageTitle,
    CategoryVNav,
    CategoryItem,
    BookItem,
  },
  data() {
    return {
      page: {
        title: "Browse Inventory",
      },
      categories: [
        {
          genre: "Fiction",
          title: "Classics",
          href: "#",
          image: fictionClassics,
          imageAlt: "Classic Fiction Canvas",
        },
        {
          genre: "Fiction",
          title: "Mystery",
          href: "#",
          image: fictionMystery,
          imageAlt: "Mysterious Lamp Canvas",
        },
        {
          genre: "How To",
          title: "Home DIY",
          href: "#",
          image: howToHomediy,
          imageAlt: "Mechanical Parts Canvas",
        },
      ],
      books: [
        {
          title: "Gaia's Garden",
          href: "#",
          author: "Toby Hemenway",
          image: bookGaia,
          imageAlt: "Gaia's Garden Floral Book Cover",
          free_read: false,
        },
        {
          title: "Bookcases, Cabinets, & Built-Ins",
          href: "#",
          author: "Fine Woodworking (editor)",
          image: bookBookcases,
          imageAlt: "Bookcases Cabinets and Built-ins Book Cover",
          free_read: false,
        },
        {
          title: "Computer Science Illuminated",
          href: "#",
          author: "Nell B Dale",
          image: bookIlluminated,
          imageAlt: "Computer Science Illuminated Book Cover",
          free_read: false,
        },
        {
          title: "Computer Science Illuminated",
          href: "#",
          author: "Nell B Dale",
          image: bookIlluminated,
          imageAlt: "Computer Science Illuminated Book Cover",
          free_read: false,
        },
        {
          title: "Computer Science Illuminated",
          href: "#",
          author: "Nell B Dale",
          image: bookIlluminated,
          imageAlt: "Computer Science Illuminated Book Cover",
          free_read: false,
        },
      ],
    };
  },
};
</script>

<style scoped>
.content_container {
  width: 100%;
}
</style>
