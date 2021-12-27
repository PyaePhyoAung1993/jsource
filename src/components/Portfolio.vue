<template>
  <v-container justify="center">
    <v-row class="justify-center">
      <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolores iure
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolores iure
          ill
        </p>
      </v-col>
      <v-col lg="12">
        <div class="text-center">
          <v-chip
            @click="activePortfolio = 'webapp'"
            :color="activePortfolio == 'webapp' ? 'success' : ''"
            class="mx-5"
            >Web App</v-chip
          >
          <v-chip
            @click="activePortfolio = 'androidapp'"
            :color="activePortfolio == 'androidapp' ? 'success' : ''"
            class="mx-5"
            >Android App</v-chip
          >
          <v-chip
            @click="activePortfolio = 'desktopapp'"
            :color="activePortfolio == 'desktopapp' ? 'success' : ''"
            class="mx-5"
            >Desktop App</v-chip
          >
        </div>
      </v-col>

      <v-col lg="3" v-for="(web, index) in webs" :key="index">
        <v-card>
          <v-img
            :src="web.image"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px"
          >
            <v-card-title>{{ web.title }}</v-card-title>
          </v-img>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Portfolio",
  data() {
    return {
      activePortfolio: "webapp",
      webs: [{ title: "App 1", image: "" }],
    };
  },
};
</script>

<style>
</style>