<template>
  <div>
    <img :src="card.thumb" :alt="card.type">
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

</style>