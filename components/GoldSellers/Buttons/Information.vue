<template>
  <div class="info-shadow d-flex justify-content-center align-item-center p-2 mb-2" dir="rtl">
    <b-row class="w-100">
      <b-col
        v-for="(item, index) in info"
        :key="index"
        cols="12"
        md="6"
        lg="4"
        xl="3"
        class="information-style"
      >
        <b-button class="btn-style p-2">
          <b-row>
            <b-col cols="2">
              <b-img :src="item.icon" class="img-style" />
            </b-col>
            <b-col>
              {{ item.name }}
            </b-col>
          </b-row>
        </b-button>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      info: [
        {
          name: 'خدمات الکترونیک',
          icon: require('@/assets/goldSeller/Asset 2.png'),
        },
        {
          name: 'جستجو واحد های صنفی',
          icon: require('@/assets/goldSeller/Asset 15.png'),
        },
        {
          name: 'قوانین و مقررات نظام صنفی',
          icon: require('@/assets/goldSeller/Asset 10.png'),
        },
        {
          name: 'بخش نامه ها و دستورالعمل ها',
          icon: require('@/assets/goldSeller/Asset 5.png'),
        },
        {
          name: 'عضویت واحدهای صنفی',
          icon: require('@/assets/goldSeller/Asset 19.png'),
        },
        {
          name: 'جستجوی مجامع و اتحادیه ها',
          icon: require('@/assets/goldSeller/Asset 14.png'),
        },
        {
          name: 'راهنمای صدور پروانه',
          icon: require('@/assets/goldSeller/Asset 9.png'),
        },
        {
          name: 'ثبت نام آموزش آنلاین',
          icon: require('@/assets/goldSeller/Asset 4.png'),
        },
        {
          name: 'تمدید و صدور پروانه',
          icon: require('@/assets/goldSeller/Asset 18.png'),
        },
        {
          name: 'ثبت شکایات/پیشنهادات/ انتقادات',
          icon: require('@/assets/goldSeller/Asset 12.png'),
        },
        {
          name: 'سیستم کاریابی',
          icon: require('@/assets/goldSeller/Asset 8.png'),
        },
        {
          name: 'ورود به منوی کاربردی',
          icon: require('@/assets/goldSeller/Asset 3.png'),
        },
        {
          name: 'مجوز فروش فوق العاده',
          icon: require('@/assets/goldSeller/Asset 16.png'),
        },
        {
          name: 'آمار و گزارشات واحدهای صنفی',
          icon: require('@/assets/goldSeller/Asset 13.png'),
        },
        {
          name: 'دستورالعمل مالیات',
          icon: require('@/assets/goldSeller/Asset 6.png'),
        },
      ],
    }
  },
}
</script>

<style scoped>
.info-shadow{
  box-shadow: 0px 5px 8px rgba(128, 128, 128, 0.927);
}

.btn-style {
  background-color: #f1f1f2;
  border-color: #f1f1f2;
  color: #c49a6c;
  margin: 2px;
  box-shadow: 5px 8px 5px rgba(128, 128, 128, 0.834);
  border-radius: 12px;
  width: 65%;
  font-family: 'B nazanin';
  font-size: 15px;
  text-align: end;
}

.information-style {
  display: flex;
  justify-content: center;
  align-items: center;
}

.img-style {
  /* width: 20px; */
  height: 25px;
}
</style>
