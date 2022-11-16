<script>
  export default {
    name: 'AppSlider'
  }
</script>


<template>
  <div class="slider">
    <div class="container">
      <div>
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <span>Digital Comics</span>
      </div>
      <div>
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <span>DC Merchandise</span>
      </div>
      <div>
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <span>Comic Shop Locator</span>
      </div>
      <div>
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <span>Subscription</span>
      </div>
      <div>
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <span>DC Power Visa</span>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.slider{
  height: 150px;
  background-color: #0D69F6;
  .container{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    img{
      height: 45px;
      vertical-align: middle;
      margin-right: 15px;
    }
    span{
      text-transform: uppercase;
      color: white;
      font-size: .8rem;
    }
  }
}
</style>