<template>
   <div id="Home">
      <div class="home">
         <div class="wrapper-home">
            <div class="container">
               <div class="row justify-content-center">
                  <div class="col-10 text-center p-5">
                     <SearchBlock></SearchBlock>
                  </div>

               </div>
            </div>
         </div>

      </div>

   </div>
</template>

<script>
 import SearchBlock from "~/components/Home/Search-Block.vue";

 export default {
    name: "Home",
    data() {
       return {

      }
    },

    components: {
      SearchBlock
    }
 }
</script>

<style scoped>

</style>
