<template>
<div class="jumbo">
  <div class="container">
    <div class="jumbo-pics">
      <ul>
        <li>
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <a href="#">Digital Commics</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <a href="#">Digital Commics</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <a href="#">Digital Commics</a>
        </li>
        <li>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <a href="#">Digital Commics</a>
        </li>
        <li>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <a href="#">Digital Commics</a>
        </li>
      </ul>
    </div>


  </div>
</div>

</template>

<script>
export default {
  name: 'JumboComp'

}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

.jumbo{
  height: 150px;
  background-color: $blue-dc;

}

.jumbo-pics{
  display: flex;
  ul{
    display: inline-flex;
    img{
      height: 80px;
    }
  }
}

</style>