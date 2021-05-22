<template>
  <main>
    <ul>
      <li>
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        Digital Comics
        </li>
      <li>
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        DC Merchandise
      </li>
      <li>
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        Subscription
      </li>
      <li>
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        Comic shop locator
      </li>
      <li>
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        DC power visa
      </li>
    </ul>
  </main>
</template>

<script>
export default {
  
}
</script>

<style lang="scss">
  main{
    width: 100%;
    height: 90px;
    padding: 0% 6%;
    background-color: #0282F9;
    display: flex;
    align-items: center;
    ul{
      width: 100%;
      display: flex;
      li{
        width: calc(100% /5);
        display: flex;
        align-items: center;
        font-size: 15px;
        color: white;
        img{
          height: 35px;
          margin-right: 10px;
        }
      }
    }
  }
</style>