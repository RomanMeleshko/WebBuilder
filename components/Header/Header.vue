<template>
  <div id="Header">
     <div class="header">
        <div class="wrapper-header">

           <nav class="navbar navbar-light bg-light">
              <a class="navbar-brand justify-content-start" href="#">WebBuilder</a>
              <div class="buttons m-auto pr-lg-5 pr-md-5">
                 <nuxt-link exact no-prefetch class="border btn btn-primary p-2" to="/Home">
                   Go to Home page
                 </nuxt-link>

                 <nuxt-link exact class="border btn btn-primary p-2" to="/Todos">
                   Go to Todos page
                 </nuxt-link>

              </div>
           </nav>

        </div>
     </div>
  </div>
</template>

<script>

 export default {
   name: "Header",
   data() {
     return {

     }
   }
 }

</script>

<style scoped>

</style>
