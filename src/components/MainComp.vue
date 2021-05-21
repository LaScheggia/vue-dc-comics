<template>
  <main class="main-bg">
    <div class="container">

      <div class="comics-card">
        <comics-card 
        v-for="(comic, index) in comics" 
        :key="index"
        :card="comic"
        />

        <h1 
        v-for="(comic, index) in comics" 
        :key="index">
          {{ comic.series }}
        </h1>
      </div>

    </div>

  </main>
</template>

<script>
// ^ importo il file js che era json
import comics from "@/assets/data/dc-comics.js";
// . importo la componente "comics card" che dentro ha il collegamento a dc.js
import ComicsCard from "@/components/ComicsCard";

export default {
  name: 'Main',
  components: {
    ComicsCard //qua lo inizializzo
  },
  data(){
    return{
      comics
    }
  },
  mounted(){
    console.log(comics)

  },
}
</script>



<style lang="scss" scoped>
.main-bg{
  padding: 50px 0;
  color: bisque;
  background-color: black;
  
}

.comics-card{
  display: flex;
  flex-wrap: wrap;
}



</style>