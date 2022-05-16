<template>
  <div class="content">
    <div class="home">
    <h1>Home</h1>
    </div>
    <!-- <select name="sort" v-model="sort">
      <option value="updatedAt:desc">Newest</option>
      <option value="price:asc">Price: Ascending</option>
      <option value="price:desc">Price: Descending</option> 
       </select> -->
  </div>
</template>

<script>
import qs from "qs";
import { ref } from 'vue';
export default {
  name: "Home",
  setup() {
   const sort = ref("updatedAt:desc");
   return {
     sort,
   }
  },
};
</script>

<style scoped>
.content{
  margin: 0 auto;
  width: 1320px; 
}
.home{
 color: rgb(0, 0, 0);
 display: flex;
 justify-content: center;
 border: 4px solid white;
 background-color: whitesmoke ;
}
</style>