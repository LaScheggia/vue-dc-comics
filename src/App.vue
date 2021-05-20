<template>
  <div id="app">
    <header-comp/>
    <main-comp/>
    <footer-comp/>


  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
  }
}
</script>


<style lang="scss">
// . GENERAL
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

// le liste in general xkè vale su tutte
ul{
  list-style: none;
}

a{
  text-decoration: none;
}

// ^ UTILITIES
// container lo vado a mettere in tutti i div di tutti i mod xkè è generico 
.container{
  display: flex;
  width: 65%;
  margin: 0 auto;
}

</style>
