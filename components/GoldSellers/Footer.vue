<template>
  <div class="footer d-flex justify-content-center align-item-center">
    <b-row
      class="w-100 px-2 d-flex justify-content-center align-item-center footer-space"
    >
      <b-col cols="12" md="4" lg="4">
        <b-row class="w-100">
          <b-col cols="12" class="link">
            <h5>دسترسی سریع</h5>
          </b-col>
          <b-col cols="12" class="link">
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              تماس با ما

            </p>
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              درباره ما

            </p>
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              نمودار سازمانی

            </p>
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              هیئت مدیره

            </p>
          </b-col>
        </b-row>
      </b-col>

      <b-col cols="12" md="4" lg="4">
        <b-row class="w-100">
          <b-col cols="12" class="link">
            <h5>لینک های مرتبط</h5>
          </b-col>
          <b-col cols="12" class="link">
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              دبیرخانه هیات عالی نظارت بر سازمان های صنفی کشور
            </p>
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              درگاه ملی مجوزهای کشور
            </p>
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              سامانه ثبت نام کلاس آموزش اتاق اصناف تهران
            </p>
            <p>
              <b-img src="@/assets/goldSeller/Asset 30.png" />
              اتاق اصناف ایران
            </p>
          </b-col>
        </b-row>
      </b-col>

      <b-col cols="12" md="4" lg="4">
        <b-row class="w-100">
          <b-col cols="12" class="link">
            <h5>نشانی</h5>
          </b-col>
          <b-col cols="12" class="address">
            <p>تهران ،خیابان سهروردی جنوبی ،خیابان شهید ملایری ،پلاک 53</p>
            <p>کد پستی: 1579713811</p>
            <p>تلفن : 88829623 - 88836342 - 88832461 -883021111</p>
            <p>88829356 - 88836340 - 88836341 -88811476</p>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.footer {
  background-image: linear-gradient(#ffffff, #f2e4d0, #f2e4d0);
}

.address {
  display: flex;
  align-items: start;
  justify-content: center;
  flex-direction: column;
  text-align: start;
}

.link {
  display: flex;
  align-items: start;
  justify-content: center;
  flex-direction: column;
  text-align: start;
}

p,
h5 {
  font-family: 'Traffic';
  color: #58595a;
}

@media (max-width: 768px) {
  p {
    font-size: 12px;
  }
  h5 {
    font-size: 14px;
  }
  /* .link {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
} */
}

@media (max-width: 425px) {
  /* .link,.address {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
} */
}

.footer-space {
  margin-top: 150px;
}
</style>
