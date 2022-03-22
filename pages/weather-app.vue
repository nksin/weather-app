<template>
  <div>
    <v-container>
      <!-- <v-layout> -->
        <h1 class="text-h4 text-center">Weather App</h1>
        <v-flex xs12>
          <v-card color="#455A64" dark>
            <v-card-text>
              here card
            </v-card-text>
          </v-card>
        </v-flex>
        <v-flex xs12 class="mt-4">
          <v-text-field
            label="enter city name" solo
          ></v-text-field>
        </v-flex>
      <!-- </v-layout> -->
    </v-container>
    </div>
</template>

<script>
export default {
  data(){
    return{
      city:'London'
    }
  },
  created(){
    this.$axios
    .$get(`https://api.openweathermap.org/data/2.5/weather?q=${this.city}&
    appid=ddb956415e4c89646c1fe66f214ec94a`)
    .then(res => console.log(res))  }

}
</script>

<style>

</style>