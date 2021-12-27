<template>
  <v-app>
    <Header></Header>
    <Herocomponent></Herocomponent>
    <About></About>
    <Portfolio></Portfolio>
    <v-main> </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import Herocomponent from "./components/Herocomponent.vue";
import About from "./components/About.vue";
import Portfolio from "./components/Portfolio.vue";

export default {
  name: "App",

  components: { Header, Herocomponent, About, Portfolio },
};
</script>
