<template>
  <div>
    <div class="header-link-mobile">
      <!-- Navbar-->
      <nav class="navbar navbar-light amber lighten-4">
        <!-- Navbar brand-->
        <a class="navbar-brand" href="#"><img src="../img/footer.png"></a>
        <!-- Collapse button-->
        <button class="navbar-toggler first-button" type="button" data-toggle="collapse" data-target="#navbarSupportedContent20" aria-controls="navbarSupportedContent20" aria-expanded="false" aria-label="Toggle navigation">
          <div class="animated-icon1">
            <span></span>
            <span></span>
            <span></span>
          </div>
        </button>
        <!-- Collapsible content-->
        <div class="collapse navbar-collapse" id="navbarSupportedContent20">
          <!-- Links-->
          <ul class="navbar-nav mr-auto">
            <li class="nav-item" v-for="item in navbarItems" :key="item"><a class="nav-link" :href="item.href" target="_blank">{{item.label}}</a></li>
<!--            <li class="nav-item"><a class="nav-link" href="https://regist.xn&#45;&#45;b3caa1e2a7e2b0h2be.com/Register/" target="_blank">ลงทะเบียนเข้าร่วมมาตรการ</a></li>-->
<!--            <li class="nav-item"><a class="nav-link" href="https://www2.xn&#45;&#45;b3caa1e2a7e2b0h2be.com/howto-register" target="_blank">ขั้นตอนการเข้าร่วม</a></li>-->
<!--            <li class="nav-item"><a class="nav-link" href="https://www2.xn&#45;&#45;b3caa1e2a7e2b0h2be.com/thung-ngern-shop-province" target="_blank">ร้านค้าที่เข้าร่วม</a></li>-->
          </ul>
        </div>
      </nav>
    </div>
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <ul class="header-links">
            <li v-for="item in navbarItems" :key="item"><a :href="item.href" target="_blank">{{item.label}}</a></li>
          </ul>
          <ul class="header-links" v-if="navbarItems.length==0">
            <li><a href="https://regist.xn--b3caa1e2a7e2b0h2be.com/Register/" target="_blank">ลงทะเบียนเข้าร่วมมาตรการ</a></li>
            <li><a href="https://www2.xn--b3caa1e2a7e2b0h2be.com/howto-register" target="_blank">ขั้นตอนการเข้าร่วม</a></li>
            <li><a href="https://www2.xn--b3caa1e2a7e2b0h2be.com/thung-ngern-shop-province" target="_blank">ร้านค้าที่เข้าร่วม</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import axios from 'axios';

  export default {
    name: "Header",
    data: function () {
      return {
        navbarItems : [],
      }
    },
    mounted () {
      axios.get('https://panjs.com/ywc.json')
        .then(response => {
          this.navbarItems = response.data.navbarItems
        })
    }
  }
</script>

<style scoped>
  {
    box-shadow: 0 4px 10px 0 rgba(0, 0, 0, 0.1);
    position: fixed;
    z-index: 200;
    width: 100%;
    height: 60px;
    max-width: none !important;
    padding: 0px;
    margin-bottom: 60px;
    background-color: #fff;
  }
  .header-links {
    list-style: none;
    margin: 0;
    padding: 5px 0 0;
    text-align: center;
  }
  @media (max-width: 577px) {
    .header-links {
      display: none;
    }
  }
  .header-links li {
    display: inline-block;
    padding: 14px 15px;
    font-family: TATSanaChon;
    font-size: 14px;
    font-weight: bold;
  }
  .header-links li a {
    text-decoration: none;
    color: #333333;
    font-weight: bold;
    background-color: transparent;
    cursor: pointer;
    position: relative;
  }
  .header-links li a:hover {
    color: #213A8F;
  }
  .header-links li a:after {
    content: "";
    position: absolute;
    width: 100%;
    height: 6px;
    bottom: -14px;
    left: 0;
    background-color: #213A8F;
    visibility: hidden;
    -webkit-transform: scaleX(0);
    transform: scaleX(0);
    -webkit-transition: all 0.3s ease-in-out 0s;
    transition: all 0.3s ease-in-out 0s;
  }
  @media (max-width: 769px) {
    .header-links li a:after {
      visibility: hidden;
    }
  }
  @media (max-width: 577px) {
    .header-links li a:after {
      visibility: hidden;
    }
  }
  .header-links li a:hover:after {
    visibility: visible;
    -webkit-transform: scaleX(1);
    transform: scaleX(1);
  }
  @media (max-width: 769px) {
    .header-links li a:hover:after {
      -webkit-transform: scaleX(0);
      transform: scaleX(0);
    }
  }
  @media (max-width: 577px) {
    .header-links li a:hover:after {
      -webkit-transform: scaleX(0);
      transform: scaleX(0);
    }
  }
  .header-link-mobile {
    display: none;
    text-align: right;
    cursor: pointer;
  }
  @media (max-width: 577px) {
    .header-link-mobile {
      display: block;
    }
  }
</style>