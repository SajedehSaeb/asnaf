<template>
  <div class="services-wrap my-3">
    <img
      :src="require('@/assets/images/asnaf/service-back.png')"
      class="back1"
    />
    <div class="wrap">
      <b-row class="justify-content-between flex-wrap">
        <div class="category1">
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category1"
              :key="index"
            >
              <img :src="require(`@/assets/images/asnaf/${item.id}.png`)" />
              <span>{{ item.title }}</span>
            </div>
          </div>
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category2"
              :key="index"
            >
              <img :src="require(`@/assets/images/asnaf/${item.id}.png`)" />
              <span>{{ item.title }}</span>
            </div>
          </div>
        </div>
        <div class="wrap-line">
          <div class="line"></div>
        </div>
        <div class="category2">
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category3"
              :key="index"
            >
              <img :src="require(`@/assets/images/asnaf/${item.id}.png`)" />
              <span>{{ item.title }}</span>
            </div>
          </div>
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category4"
              :key="index"
            >
              <img :src="require(`@/assets/images/asnaf/${item.id}.png`)" />
              <span>{{ item.title }}</span>
            </div>
          </div>
        </div>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ServicesComponent',
  data() {
    return {
      category1: [
        { title: 'خدمات الکترونیک', id: 1 },
        { title: 'عضویت واحدهای صنفی', id: 2 },
        { title: 'تمدید و صدور پروانه', id: 3 },
        { title: 'مجوز فروش فوق العاده', id: 4 },
      ],
      category2: [
        { title: 'جستجوی واحدهای صنفی', id: 5 },
        { title: 'جستجوی مجامع و اتحادیه ها', id: 6 },
        { title: 'ثبت شکایات / پیشنهادات / انتقادات', id: 7 },
        { title: 'آماروگزارشات واحدهای صنفی', id: 8 },
      ],
      category3: [
        { title: 'قوانین و مقررات نظام صنفی', id: 9 },
        { title: 'راهنمای صدور پروانه', id: 10 },
        { title: 'سیستم کاریابی', id: 11 },
        { title: 'دستورالعمل مالیات', id: 12 },
      ],
      category4: [
        { title: 'بخش نامه ها و دستورالعمل ها', id: 13 },
        { title: 'ثبت نام آموزش آنلاین', id: 14 },
        { title: 'ورود به منوی کاربردی', id: 15 },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.services-wrap {
  position: relative;
  .back1 {
    position: absolute;
    left: 0;
    top: 0;
  }
  .wrap {
    width: 83%;
    margin: 0 auto;
    .category1 {
      width: 45%;
      display: flex;
      justify-content: space-between;
      font-family: 'B nazanin';
      @media screen and (max-width: 992px) {
        width: 100%;
      }
      @media screen and (max-width: 500px) {
        flex-direction: column;
      }
    }
    .category2 {
      width: 45%;
      display: flex;
      justify-content: space-between;
      font-family: 'B nazanin';
      @media screen and (max-width: 992px) {
        width: 100%;
      }
      @media screen and (max-width: 500px) {
        flex-direction: column;
      }
    }
    .wrap-line {
      width: 5%;
      display: flex;
      justify-content: center;

      .line {
        width: 1px;
        height: 100%;
        border: 1px dashed rgba(128, 128, 128, 0.781);
      }
      @media screen and (max-width: 992px) {
        display: none;
      }
    }
    .service {
      width: 40%;
      @media screen and (max-width: 500px) {
        width: 100%;
      }
      .single {
        text-align: right;
        color: #2b3990;
        background-color: #f1f2f2;
        border-radius: 15px;
        -webkit-box-shadow: 8px 9px 12px 0px rgba(125, 123, 125, 1);
        -moz-box-shadow: 8px 9px 12px 0px rgba(125, 123, 125, 1);
        box-shadow: 8px 9px 12px 0px rgba(125, 123, 125, 1);
        img {
          width: 45px;
          height: 50px;
        }
        span {
          font-size: 15px;
        }
      }
    }
  }
}
</style>
