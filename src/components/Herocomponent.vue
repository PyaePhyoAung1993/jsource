<template>
  <v-container class="mt-15">
    <v-row>
      <v-col lg="6">
        <h2 class="introtext">Welcome to My Website</h2>
        <p class="description">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fugiat
          impedit magni quis quas laudantium maxime, laborum omnis aliquid hic
          voluptas veniam natus debitis iusto ut. Quia veniam provident iste
          sit?
        </p>
        <v-btn color="success" class="white--text" rounded>Get Started</v-btn>
        <v-btn color="indigo" class="white--text ml-15" rounded>
          <v-icon>mdi-play-circle</v-icon>
          Watch video</v-btn
        >
      </v-col>
      <v-col lg="6">
        <v-card>
          <img width="560" src="./../assets/coding-man.jpg" alt="" />
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Herocomponent",
};
</script>

<style scoped>
h2.introtext {
  font-size: 60px;
  font-weight: bold;
  font-family: cursive;
  color: #444;
}
p.description {
  font-size: 19px;
  font-family: cursive;
  color: #444444ba;
}
</style>