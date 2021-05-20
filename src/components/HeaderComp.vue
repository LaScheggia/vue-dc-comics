<template>
<header class="container">
  <!-- LOGO -->
  <div class="head-logo">
    <a href="/">
      <img src="../assets/img/dc-logo.png" alt="logo png">
    </a>
  </div>

<!-- NAVBAR -->
  <div class="head-nav">
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
@import '../assets/style/vars.scss';

header{
  height: 120px;
  display: flex;
  align-items: center;
}


.head-logo{
  width: 35%;
}

.head-nav{
  width: auto;
  nav{
    width: 100%;
  }
}

ul{
  display: flex;
  width: 100%;
  justify-content: right;
  margin: 2rem 0;
  font-size: 0.85rem;
  a{
    padding: 1rem;
    color: rgb(79, 76, 72);
    text-transform: uppercase;
    &:hover,
    &.active{
      padding-bottom: 48px;
      border-bottom: 5px solid $blue-dc;
    }
  }
}







  

</style>