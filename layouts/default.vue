<template>
<v-app>
  <v-main>
  
  <v-toolbar>
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <v-toolbar-title>portfolio</v-toolbar-title>

    <v-spacer></v-spacer>

    <v-btn text>
      <n-link id="brown" to="/weather-app">weather app</n-link>
    </v-btn>
  </v-toolbar>
  <v-main>
    <nuxt/>
  </v-main>
  </v-main>
  </v-app>
</template>

<script>
export default {

}
</script>

<style>

#brown{
  text-decoration: none;
  color: rgb(255, 255, 255);
}

</style>