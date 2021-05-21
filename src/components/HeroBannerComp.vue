<template>
  <div class="hero">

    <div class="container">
      <button>
        CURRENT SERIES
      </button>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'HeroBannerComp',

}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

.hero{
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  height: 350px;
}

button{
  background-color: $blue-dc;
  padding: 10px 20px;
  border: 0;
  color: white;
  font-weight: bolder;
  &:hover{
    background-color: rgb(20, 83, 143);
  }
}

</style>