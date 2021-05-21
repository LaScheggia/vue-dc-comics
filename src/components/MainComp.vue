<template>
  <main class="main-bg">
    <div class="container">
      <h1>
        CONTENT GOES HERE -->
      </h1>
    </div>

  </main>
</template>

<script>
import comics from "@/assets/data/dc-comics.js";
import ComicsCard from "@/components/ComicsCard";

export default {
  name: 'Main',
  components: {
    ComicsCard
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


</style>