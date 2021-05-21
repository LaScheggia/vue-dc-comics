<template>
  <div>
    <img 
    :src="card.thumb"  
    :alt="card.type">
  </div>
</template>

<script>
export default {
  name:'ComicsCard',
  props:{
    card: Object
  }

}
</script>

<style lang="scss" scoped>
div{
  display: flex;
  flex-basis: calc(100% / 7);
  img{
    width: 200px;
    height: 200px;
  }
}

</style>