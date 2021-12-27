<template>
  <v-app-bar app color="white" light style="padding: 0px 90px">
    <v-toolbar-title> Jsource </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-list class="d-flex align-center">
      <v-list-item
        link
        v-for="(menu, index) in menus"
        :key="index"
        :to="menu.route"
      >
        <v-list-item-title>{{ menu.title }}</v-list-item-title>
      </v-list-item>
      <v-btn text class="mx-15">
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-btn outlined color="success">Get Started</v-btn>
    </v-list>
  </v-app-bar>
</template>

<script>
import AboutVue from "./About.vue";
import ContactVue from "./Contact.vue";
import GalleryVue from "./Gallery.vue";
import PortfolioVue from "./Portfolio.vue";
import ProjectVue from "./Project.vue";
export default {
  name: "Header",
  data: () => ({
    menus: [
      { title: "Home", route: "Home" },
      { title: "About", route: AboutVue },
      { title: "Protfolio", route: PortfolioVue },
      { title: "Project", route: ProjectVue },
      { title: "Gallery", route: GalleryVue },
      { title: "Contact", route: ContactVue },
    ],
  }),
};
</script>

<style scoped>
.v-toolbar__title {
  font-size: 32px;
  font-weight: 700;
  color: #4caf50;
  font-family: cursive;
}
</style>