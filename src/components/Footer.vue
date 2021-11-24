<template>
  <footer>

    <div class="footer__top">
      <div class="container">

        <div class="col">
          <ul>
            <li><h3>DC COMICS</h3></li>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <ul>
            <li><h3>DC SHOP</h3></li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <li><h3>DC</h3></li>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policy (New)</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <li><h3>SITES</h3></li>
            <li><a href="#">DC</a></li>
            <li><a href="#">DC UNIVERSE INFINITE</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Shop</a></li>
            <li><a href="#">MAD Magazine</a></li>
          </ul>
        </div>
        <div class="col-img">
          <img src="../assets/img/dc-logo-bg.png" alt="Logo DC">
        </div>

      </div>
    </div>

    <div class="footer__bottom">
      <div class="footer__bottom_left">
        <div class="button">
          <a href="#">SIGN-UP NOW!</a>
        </div>
      </div>
      <div class="footer__bottom_right">
          <span>FOLLOW US</span>
      </div>
    </div>

  </footer> 
</template>

<script>
export default {
  name: 'Footer'

}
</script>

<style lang="scss">

@import "../assets/style/vars.scss";

.footer__top {
  background-image: url(../assets/img/footer-bg.jpg);
  max-height: 350px;
  overflow: hidden;
  padding: 40px 0;
  .container {
    display: flex;
    .col {
      margin-right: 50px;
      ul {
        margin-bottom: 15px;
        h3 {
          color: #fff;
          margin-bottom: 10px;
          font-size: 18px;
        }
        a {
          font-size: 11px;
          &:hover {
          color: $primary-color;
        }
        }
      }
    }
    .col-img {
      margin-left: 50px;
      img {
        width: 500px;
        margin-top: -120px;
      }
    }
  }
}

.footer__bottom {
  display: flex;
  justify-content: space-between;
  padding: 40px;
  background-color: #303030;
}

</style>