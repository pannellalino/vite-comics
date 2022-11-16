<script>
  export default {
    name: 'AppFooter'
  
  }
</script>


<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <nav>
          <div class="col">
            <h3>DC Comics</h3>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h3>Shop</h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col">
            <h3>DC</h3>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="col">
            <h3>Sites</h3>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </nav>
        <div class="logo">
        </div>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="container">
        <div class="button">
          <button><a href="#">SIGN-UP NOW!</a></button>
        </div>
        <div class="icons">
          <h3>FOLLOW US</h3>
          <img src="../assets/img/footer-facebook.png" alt="fb">
          <img src="../assets/img/footer-periscope.png" alt="fb">
          <img src="../assets/img/footer-pinterest.png" alt="fb">
          <img src="../assets/img/footer-twitter.png" alt="fb">
          <img src="../assets/img/footer-youtube.png" alt="fb">
        </div>
      </div>
    </div>
  </footer>
</template>


<style lang="scss" scoped>
footer{
  .footer-top{
    height: 400px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    .container{
      height: 100%;
      display: flex;
      justify-content: space-between;
      background-image: url('../assets/img/dc-logo-bg.png');
      background-repeat: no-repeat;
      background-position: center right;
    }
    nav{
      display: flex;
      margin: 30px 0;
      .col{
        margin-right: 40px;
      }
    }
    h3{
      color: white;
      text-transform: uppercase;
      margin-bottom: 10px;
    }
    ul{
      margin-bottom: 10px;
      li{
        list-style: none;
        a{
          text-decoration: none;
          font-size: .8rem;
          color: #858483;
        }
      }
    }
  }
  .footer-bottom{
    height: 120px;
    background-color: #242424;
    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100%;
      button{
        border: 1px solid #0D6EFF;
        background-color: transparent;
        padding: 10px;
        &:hover{
          border: 1px solid #242424;
          background-color: #0D6EFF;
        }
        a{
          color: white;
          text-decoration: none;
        }
      }
    }
    .icons{
      display: flex;
      align-items: center;
      h3, img{
        margin: 10px;
      }
      h3{
        color: #0D6EFF;
      }
    }
  }
}
</style>