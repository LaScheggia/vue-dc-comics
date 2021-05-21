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
@import '../assets/style/mixins.scss';

.hero{
  background-image: url(../assets/img/jumbotron.jpg);
  background-size: cover;
  height: 350px;
}

button{
  @include btn-dc;

}

</style>