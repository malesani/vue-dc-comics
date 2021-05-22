<template>
  <footer>
    <div class="footer-menu">
      <ul class="f-menu-1">
        <ul>
          <h3>DC Comics</h3>
          <li>Characters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
        </ul>
        <ul>
          <h3>Shop</h3>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>
      </ul>

      <ul class= "f-menu-2">
        <h3>DC</h3>
        <li>Terms Of Use</li>
        <li>Privacy policy (New)</li>
        <li>Ad Choises</li>
        <li>Advertising</li>
        <li>Jobs</li>
        <li>Subscriptions</li>
        <li>Talent Workshops</li>
        <li>CPS Certificates</li>
        <li>Ratings</li>
        <li>Shop Help</li>
        <li>Contact Us</li>
      </ul>

      <ul class="f-menu-3">
        <h3>Sites</h3>
        <li>DC</li>
        <li>MAD Magazine</li>
        <li>DC Kids</li>
        <li>DC Universe</li>
        <li>Dc Power Visa</li>
      </ul>
      <img src="../assets/img/dc-logo-bg.png" alt="">
    </div>
    <div class="footer-social">
      <button>SIGN-UP NOW!</button>
      <ul>
        <li>FOLLOW US</li>
        <li><img src="../assets/img/footer-facebook.png" alt=""></li>
        <li><img src="../assets/img/footer-twitter.png" alt=""></li>
        <li><img src="../assets/img/footer-youtube.png" alt=""></li>
        <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
        <li><img src="../assets/img/footer-periscope.png" alt=""></li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  
}
</script>
  
<style lang="scss">
  footer{
    .footer-menu{
      height: 295px;
      background-image: url(../assets/img/footer-bg.jpg);
      display: flex;
      padding: 3% 10%;
      position: relative;
      overflow: hidden;
      
      
      ul{
        width: 120px;
        color: white;
        margin-right: 25px;
        margin-bottom: 20px;
        h3{
          margin-bottom: 10px;
        }
        li{
          font-size: 10px;
          padding-bottom: 5px;
          color: #919190;
        }
      }
      img{
        height: 400px;
        position: absolute;
        top: -70px;
        right: 230px;
        overflow:hidden;
       
      }
    }
    .footer-social{
      height: 80px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #303030;
      padding: 0% 10%;

      button{
        height: 35px;
        padding: 10px;
        border: solid #0282F9 2px;
        color: white;
        background-color: #303030;
      }
      ul{
        display: flex;
        align-items: center;
        li{
          color: #0282F9;
          margin-right: 15px;
          img{
            height: 25px;
          }
        }
      }
    }
  }
</style>