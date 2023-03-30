<template>
  <div id="Home">
    <div class="Home">
      <div>
        <Welcome></Welcome>
      </div>

    </div>
  </div>
</template>

<script>
import Welcome from "~/components/Welcome/Welcome.vue";

 export default {
    name: "Home",
    data() {
       return {

       }
    },

    component: {
      Welcome
    }
 }

</script>

<style scoped>

</style>
