<template>
  <div id="app">
    <v-app>
      <v-main>
        <Main/>
      </v-main>
    </v-app>
  </div>
</template>

<script>
import Main from './components/Main.vue'
export default {
  name: "App",

  components: {
    Main
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
#app{
  background-image:url("https://images2.alphacoders.com/238/thumb-1920-238870.jpg");
}
</style>