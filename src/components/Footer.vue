<template>
  <div>
      <div class="footer-1" style="position: relative;">
        <div class="container">
          <div class="row">
            <div class="col-md-3 col-sm-12"><img class="logo" src="../img/footer.png"></div>
            <div class="col-md-3 col-sm-4 col-xs-12">
              <div class="head">ข้อมูลลงทะเบียนประชาชน</div>
              <div class="detail">การรับสิทธิ การใช้งานแอปพลิเคชั่น <span class="nowrap">“เป๋าตัง”</span> และ <span class="nowrap">“ถุงเงิน”</span></div>
              <div class="detail">ติดต่อ ชิมช้อปใช้ Call Center by Krungthai โทร.<a class="ml-1" href="tel:021111144"><span class="nowrap">0 2111 1144</span></a></div>
            </div>
            <div class="col-md-3 col-sm-4 col-xs-12">
              <div class="head">ข้อมูลลงทะเบียนผู้ประกอบการ</div>
              <div class="detail">เงื่อนไขและวิธีการเข้าร่วมมาตรการฯ</div>
              <div class="detail">ติดต่อ โทร.<a class="ml-1" href="tel:022706400"><span class="nowrap">0 2270 6400 กด 7</span></a></div>
            </div>
            <div class="col-md-3 col-sm-4 col-xs-12">
              <div class="head">ข้อมูลเที่ยวชิมช้อปใช้</div>
              <div class="detail">ติดต่อ ททท.</div>
              <div class="detail">โทร<a class="ml-1" href="tel:1672"><span>1672</span></a></div>
            </div>
          </div>
        </div>
      </div>
      <div class="footer-2">
        <div class="container">
          <div class="row no-gutters">
            <div class="col-sm-12 col-md-3 col-lg-3">
              <div class="copyright">Copyright © 2003-2019</div>
            </div>
            <div class="row col-sm-12 col-md-9 col-lg-9">
              <ul class="nav col-sm-12">
                <li class="col-sm-4 col-md-4 col-lg-4 nav-item"><a class="nav-link" href="https://regist.xn--b3caa1e2a7e2b0h2be.com/Register/" target="_blank">ลงทะเบียนเข้าร่วมมาตรการ</a></li>
                <li class="col-sm-4 col-md-4 col-lg-4 nav-item"><a class="nav-link" href="https://www2.xn--b3caa1e2a7e2b0h2be.com/howto-register" target="_blank">ขั้นตอนการเข้าร่วมทั้งหมด</a></li>
                <li class="col-sm-4 col-md-4 col-lg-4 nav-item"><a class="nav-link" href="https://www2.xn--b3caa1e2a7e2b0h2be.com/thung-ngern-shop-province" target="_blank">รายชื่อร้านค้าที่เข้าร่วมรายการ</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
  export default {
    name: "Footer"
  }
</script>

<style scoped>
  {
    font-size: 14px;
  }
  .footer-1 {
    background-color: #FAFAFA;
    padding: 30px;
  }
  @media (max-width: 577px) {
    .footer-1 {
      padding: 44px 30px;
    }
  }
  .footer-1 .head {
    font-weight: bold;
    color: #E6332A;
    margin-top: 24px;
    font-size: 16px;
  }
  @media (max-width: 577px) {
    .footer-1 .head {
      margin: 15px 0px 10px 0px ;
    }
  }
  .footer-1 .logo {
    width: 108px;
  }
  @media (max-width: 577px) {
    .footer-1 .logo {
      width: 145px;
    }
  }
  .footer-1 a {
    text-decoration: none;
    color: #333333;
  }
  .footer-2 {
    font-family: 'TATSanaSuksaBold';
    background-color: #213A8F;
    color: #fff;
  }
  @media (max-width: 577px) {
    .footer-2 {
      padding: 15px 0px;
    }
  }
  @media (max-width: 769px) {
    .footer-2 .container {
      max-width: 100%;
    }
  }
  .footer-2 .copyright {
    padding: 0.5rem 1rem;
    padding-left: 0px;
  }
  @media (max-width: 769px) {
    .footer-2 .copyright {
      padding: 0.5rem 0.5rem;
      font-size: 12px;
    }
  }
  @media (max-width: 577px) {
    .footer-2 .copyright {
      padding: 0.5rem 2rem;
    }
  }
  .footer-2 .nav {
    float: right;
  }
  @media (max-width: 769px) {
    .footer-2 .nav .nav-link {
      padding: 0.5rem 0.5rem;
      font-size: 12px;
    }
  }
  @media (max-width: 577px) {
    .footer-2 .nav .nav-link {
      padding: 0.5rem 2rem;
    }
  }
  .footer-2 a {
    font-size: 14px;
    text-decoration: none;
    color: #fff;
  }
</style>