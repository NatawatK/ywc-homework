<template>
  <div>
    <div class="banner">
      <div class="row no-gutters">
        <div class="col-4 cover-img-1"></div>
        <div class="col-4 cover-img-2">
          <div class="row h-100 justify-content-center align-items-center">
            <div class="col-12">
              <div class="logo-box"><img src="../img/banner.png" alt="banner"></div>
            </div>
          </div>
        </div>
        <div class="col-4 cover-img-3"></div>
      </div>
    </div>
    <div class="box-register">
      <div class="container-fluid">
        <div class="row">
          <div class="col-12">
            <div class="since">ตั้งแต่วันที่</div>
          </div>
          <div class="col-12">
            <div class="time">{{duration}}</div>
            <div class="time" v-if="!duration">27 ก.ย. - 31 ธ.ค. 62</div>
          </div>
          <div class="col-12"><a href="https://regist.xn--b3caa1e2a7e2b0h2be.com/Register/" target="_blank">
            <button class="btn register">ลงทะเบียน เฟส 2<br>
              ตั้งแต่วันที่ 24 ต.ค.62 วันละ 2 รอบ เวลา 6:00 และ 18:00 น. <br>
              (จำกัดจำนวนผู้ลงทะเบียนรอบละ 5 แสนคน รวม 1 ล้านคนต่อวัน)<br>
              </button>
<!--            <hr>-->
          </a></div>
        </div>
      </div>
    </div>
    <div class="box-detail">
      <div class="container">
        <div class="row">
          <div class="col-md-10">
            <div class="row">
              <div class="col-12" style="text-align: left;">
                <div class="head-title d-none d-sm-block">มาตรการส่งเสริมการบริโภค <br> ในประเทศ <span class="nowrap">“ชิมช้อปใช้”</span></div>
                <div class="head-title d-sm-none">มาตรการส่งเสริมการบริโภคในประเทศ <span class="nowrap">“ชิมช้อปใช้”</span></div>
              </div>
              <div class="col-12 mt-4" style="text-align: left;">
                <div class="detail" v-html="detail" ></div>
<!--                <div class="detail" >ผู้สนใจเข้าร่วมมาตรการส่งเสริมการบริโภคในประเทศ <span class="nowrap">“ชิมช้อปใช้”</span> รับเงินผ่าน <span class="nowrap">“เป๋าตัง”</span> <span class="nowrap">(G-Wallet)</span> รวมจำนวน 13 ล้านคน  ลงทะเบียนรับสิทธิ ได้ทางเว็บไซต์ <span class="nowrap">www.ชิมช้อปใช้.com</span> <br> ตั้งแต่วันที่ 23 กันยายน  - 15 พฤศจิกายน 2562 (รับลงทะเบียน เฟส 2 ตั้งแต่วันที่ 24 ตุลาคม 2562 จำกัดจำนวนผู้ลงทะเบียน 1 ล้านคนต่อวัน จนกว่าจะครบ 3 ล้านคน)</div>-->
              </div>
              <div class="col-12 condition mt-4" style="text-align: left;">
                <div class="title">เงื่อนไขการเข้าร่วมมาตรการ</div>
                <div class="detail ul mt-2" v-html="condition">
<!--                  1. เป็นบุคคลสัญชาติไทย มีบัตรประจำตัวประชาชน<br>-->
<!--                  2. มีอายุตั้งแต่ 18 ปีบริบูรณ์ขึ้นไป ณ วันที่ลงทะเบียน<br>-->
<!--                  3. มีโทรศัพท์มือถือสมาร์ทโฟนที่สามารถเชื่อมต่อสัญญาณอินเทอร์เน็ตและมีอีเมล-->
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-3 col-lg-8"></div>
        </div>
      </div>
    </div>
    <div class="box-tat">
      <div class="container">
        <div class="row">
          <div class="col-sm-12 col-md-4"><a href="tel:021111144"><img src="../img/Banner_KTB_SQ.png"></a></div>
          <div class="col-sm-12 col-md-4"><a href="tel:022706400"><img src="../img/Banner_CGD_Sq.png"></a></div>
          <div class="col-sm-12 col-md-4"><a href="tel:1672"><img src="../img/Banner_TAT_Hotline_Sq.png"></a></div>
        </div>
      </div>
    </div>
    <div class="box-ktc">
      <div class="container">
        <div class="row d-none d-sm-block">
          <div class="d-flex justify-content-around">
            <div class="p2"><a href="https://www.mof.go.th/th/home" target="_blank"><img src="../img/brand_logo/MOF.png" alt="MOF logo"></a></div>
            <div class="p2"><a href="http://www.fpo.go.th/" target="_blank"><img src="../img/brand_logo/FPO.png" alt="FPO logo"></a></div>
            <div class="p2"><a href="https://www.cgd.go.th/" target="_blank"><img src="../img/brand_logo/CGD.png" alt="CGD logo"></a></div>
            <div class="p2"><a href="https://www.newcb.ktb.co.th/" target="_blank"><img src="../img/brand_logo/Krungthai.png" alt="Krungthai logo"></a></div>
            <div class="p2"><a href="https://www.mots.go.th/" target="_blank"><img src="../img/brand_logo/MOTS.png" alt="MOTS logo"></a></div>
            <div class="p2"><a href="https://thai.tourismthailand.org/" target="_blank"><img src="../img/brand_logo/TAT.png" alt="TAT logo"></a></div>
          </div>
        </div>
        <div class="row d-sm-none">
          <div class="col-4 text-right"><a href="https://www.mof.go.th/th/home" target="_blank"><img src="../img/brand_logo/MOF.png"></a></div>
          <div class="col-4 text-center"><a href="http://www.fpo.go.th/" target="_blank"><img src="../img/brand_logo/FPO.png"></a></div>
          <div class="col-4 text-left"><a href="https://www.cgd.go.th/" target="_blank"><img src="../img/brand_logo/CGD.png"></a></div>
          <div class="col-4 text-right"><a href="https://www.newcb.ktb.co.th/" target="_blank"><img src="../img/brand_logo/Krungthai.png"></a></div>
          <div class="col-4 text-center"><a href="https://www.mots.go.th/" target="_blank"><img src="../img/brand_logo/MOTS.png"></a></div>
          <div class="col-4 text-left"><a href="https://thai.tourismthailand.org/" target="_blank"><img src="../img/brand_logo/TAT.png"></a></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import axios from "axios"
  export default {
    name: "LandingPages",
    data : function () {
      return {
        duration : "",
        detail : "",
        condition : "",
      }
    },
    mounted() {
      axios.get('https://panjs.com/ywc.json')
      .then((response) => {
        this.duration = response.data.duration
        this.detail = response.data.detail
        this.condition = response.data.condition
      })
    }

  }
</script>

<style scoped>

</style>