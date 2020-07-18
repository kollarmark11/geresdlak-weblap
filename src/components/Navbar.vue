<template>
  <div class="container-fluid">
    <v-toolbar dark color="purple darken-3" app height="60">
      <v-app-bar-nav-icon>
        <img
          src="https://i.ibb.co/HVq5GSH/glak-logo.png"
          alt=""
          height="40"
          class="pl-10"
        />
      </v-app-bar-nav-icon>

      <v-toolbar-title class="d-none d-sm-flex text-uppercase pl-10"
        >Geresdlaki Dózsa Se</v-toolbar-title
      >
      <v-spacer></v-spacer>

      <v-btn text>
        <router-link to="/" id="routerlinks">Home</router-link>
      </v-btn>

      <v-divider vertical class="mx-4 d-none d-sm-flex" inset></v-divider>
      <v-btn text>
        <a href="#section" id="routerlinks">About</a>
      </v-btn>

      <v-divider vertical class="mx-4 d-none d-sm-flex" inset></v-divider>
      <v-btn text>
        <a href="#section" id="routerlinks">Contact</a>
      </v-btn>

      <v-divider vertical class="mx-4 d-none d-sm-flex" inset></v-divider>
      <v-btn text>
        <router-link to="/about" id="routerlinks" class="pa-8"
          >Gallery</router-link
        >
      </v-btn>
    </v-toolbar>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@media screen and (max-width: 600px) {
  #routerlinks {
    font-size: 15px;
  }
}
</style>
