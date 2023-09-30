<template>
  <div class="services-wrap my-3">
    <div class="wrap">
      <b-row class="justify-content-between flex-wrap">
        <div class="category">
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category1"
              :key="index"
            >
              <img
                :src="
                  require(`@/assets/images/asnaf/tehran-asnaf/${item.id}.png`)
                "
              />
              <span class="mr-1">{{ item.title }}</span>
            </div>
          </div>
        </div>

        <div class="category">
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category2"
              :key="index"
            >
              <img
                :src="
                  require(`@/assets/images/asnaf/tehran-asnaf/${item.id}.png`)
                "
              />
              <span class="mr-1">{{ item.title }}</span>
            </div>
          </div>
        </div>

        <div class="category">
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category3"
              :key="index"
            >
              <img
                :src="
                  require(`@/assets/images/asnaf/tehran-asnaf/${item.id}.png`)
                "
              />
              <span class="mr-1">{{ item.title }}</span>
            </div>
          </div>
        </div>

        <div class="category">
          <div class="service">
            <div
              class="single d-flex align-items-center mt-2"
              v-for="(item, index) in category4"
              :key="index"
            >
              <img
                :src="
                  require(`@/assets/images/asnaf/tehran-asnaf/${item.id}.png`)
                "
              />
              <span class="mr-1">{{ item.title }}</span>
            </div>
          </div>
        </div>
      </b-row>
    </div>
  </div>
</template>

  <script>
export default {
  name: 'AsnafServices',
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
  .wrap {
    width: 83%;
    margin: 0 auto;
    .category {
      width: 25%;
      padding: 0 20px;
      display: flex;
      justify-content: space-between;
      border-left: 2px dashed rgba(218, 217, 217, 0.541);
      &:last-child {
        border-left: none;
      }
      @media screen and (max-width: 992px) {
        width: 50%;
        &:nth-child(2) {
          border-left: none;
        }
      }
      @media screen and (max-width: 578px) {
        width: 100%;
        border-left: none;
      }
    }
    .service {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      .single {
        width: 70%;
        text-align: right;
        color: #2b3990;

        background-color: #f1f2f2;
        border-radius: 15px;
        -webkit-box-shadow: 8px 9px 12px 0px rgba(125, 123, 125, 1);
        -moz-box-shadow: 8px 9px 12px 0px rgba(125, 123, 125, 1);
        box-shadow: 8px 9px 12px 0px rgba(125, 123, 125, 1);
        padding: 5px;
        @media screen and (max-width: 768px) {
        width: 90%;
      }
        img {
          width: 35px;
          height: 40px;
        }
        span {
          font-size: 15px;
          color: #662D91;
          font-family: 'B nazanin';
        }
      }
    }
  }
}
</style>
