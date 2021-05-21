<template>
  <div>
    <img 
    :src="card.thumb"  
    :alt="card.type">
    <p>
      {{ card.series }}
    </p>
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
  flex-basis: calc(100% / 6);
  padding: 5px;
  img{
    width: 150px;
    height: 150px;
  }
  p{
    font-size: 0.8rem;
    text-transform: uppercase;
  }
}

</style>