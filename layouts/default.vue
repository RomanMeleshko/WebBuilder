<template>
  <div id="App">
     <nuxt />
  </div>
</template>

<script>
import Welcome from "~/components/Welcome/Welcome.vue";

 export default {
    name: "App",
    data() {
       return {

      }
    },

   components: {
      Welcome
    }
 }

</script>

<style scoped>

</style>
