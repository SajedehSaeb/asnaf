<template>
    <div class="wrap">
      <div class="content d-flex flex-column">
        <strong class="caption">پیوندهای مرتبط</strong>
        <div class="socials mt-2">
          <div v-for="(item, index) in socials" :key="index" class="d-flex mt-1">
            <h6 class="mr-2">{{ item.title }}</h6>
          </div>
        </div>
      </div>
    </div>
  </template>

    <script>
  export default {
    name: 'RelatedLinks',
    data() {
      return {
        socials: [
          { title: 'اتاق بازرگانی , صنایع , معادن وکشاورزی سازمان امور مالیاتی کشور' },
          { title: 'پایگاه اطلاع رسانی مقام معظم رهبری' },
          { title: 'پایگاه اطلاع رسانی رییس جمهور' },
          { title: 'خبرگزاری ایرنا' },
          { title: 'خبرگزاری ایسنا' },
          { title: 'خبرگزاری ایلنا' },
          { title: 'خبرگزاری فارس' },
          { title: 'خبرگزاری تسنیم' },
          { title: 'خبرگزاری مهر' },
        ],
      }
    },
  }
  </script>

    <style scoped lang="scss">
  .wrap {
    .content {
      .caption {
        font-size: 27px;
        text-align: right;
        font-family: 'B nazanin';
      }
      .socials {
        font-family: 'B nazanin';
        h6 {
          font-size: 12px;
          text-align: right;
        }
      }
    }
  }
  </style>
