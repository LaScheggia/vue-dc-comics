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

    <div class="btn">

      <button>
        CURRENT SERIES
      </button>
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
@import '../assets/style/vars.scss';
.main-bg{
  padding: 50px 0;
  color: bisque;
  background-color: black;
}

.comics-card{
  display: flex;
  flex-flow: wrap;
  align-content: space-around;
}

.btn{
  display: flex;
  background-color: whitesmoke;
}

button{

  background-color: $blue-dc;
  padding: 10px 20px;
  border: 0;
  color: white;
  font-weight: bolder;
  justify-content: center;
}


</style>