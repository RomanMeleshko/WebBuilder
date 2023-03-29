<template>
   <div class="Search-Block">
      <div class="search-block">
         <div class="wrapper-search-block">

            <div class="search-input-block">
               <textarea v-model="info_from_input" type="text" autocomplete="on" name="searcher" />
            </div>

         </div>

      </div>
   </div>
</template>

<script>

 export default {
    name: "Search-Block",
    data() {
       return {
         info_from_input: ""
       }
    },

    watch: {

       info_from_input( value ) {
         console.log( value );
       }

    }
 }
</script>

<style>

</style>
