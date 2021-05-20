<template>
<header class="container">
  <!-- LOGO -->
  <div class="cols">
    <a href="/">
      <img src="../assets/img/dc-logo.png" alt="">
    </a>
  </div>

<!-- NAVBAR -->
  <div class="cols">
    <nav>
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :class="{'active': link.current}" :href="link.url">{{link.text}}</a>
        </li>
      </ul>
    </nav>
  </div>
</header>
  
</template>

<script>
export default {
  name: 'HeaderComp',
  data(){
    return{
      links: [
        {
          text: 'Characters',
          url: '#',
          current: false
        },
        {
          text: 'Comics',
          url: '#',
          current: true
        },
        {
          text: 'Movies',
          url: '#',
          current: false
        },
        {
          text: 'Tv',
          url: '#',
          current: false
        },
        {
          text: 'Games',
          url: '#',
          current: false
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false
        },
        {
          text: 'Videos',
          url: '#',
          current: false
        },
        {
          text: 'Fans',
          url: '#',
          current: false
        },
        {
          text: 'News',
          url: '#',
          current: false
        },
        {
          text: 'Shop',
          url: '#',
          current: false
        },
      ]
    }
  }

}
</script>

<style lang="scss" scoped> // ^ abc
header{
  height: 150px;
  background-color: aquamarine;
  display: flex;
  align-items: center;
}

.cols{
  flex-basis: calc(100% / 2);
}

 ul{
   display: flex;
   justify-content: left;
   margin: 2rem 0;
   a{
     padding: 1rem;
     color: rgb(79, 76, 72);
     text-transform: uppercase;
     &:hover,
     &.active{
       border-bottom: 4px solid rgb(2, 130, 249);
     }
   }
 }

  

</style>