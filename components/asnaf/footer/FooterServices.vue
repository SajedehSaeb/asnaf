<template>
  <div class="wrap my-5">
    <div class="options d-flex flex-wrap justify-content-between">
      <div
        v-for="(option, index) in options"
        :key="index"
        class="single d-flex flex-column justify-content-center align-items-center mt-3"
      >
        <img :src="require(`@/assets/images/asnaf/footer/${index + 1}.png`)" />
        <h4 class="mt-3">{{ option.title }}</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterServices',
  data() {
    return {
      options: [
        { title: 'کتابخانه دیجیتال' },
        { title: 'بازتاب رسانه ای' },
        { title: 'انتشارات' },
        { title: 'پادکست' },
        { title: 'اینفوگرافی' },
        { title: 'نظرسنجی' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.wrap {
  width: 70%;
  margin: 0 auto;
  .options {
    .single {
      width: 16%;
      font-family: 'B nazanin';
      border-left: 2px dashed rgba(189, 188, 188, 0.658);
      color: #2b3990;
      padding: 50px 0;
      &:last-child {
        border-left: none ;
      }
      h4 {
        font-size: 20px;
        text-align: center;
      }
      @media screen and (max-width: 992px) {
        width: 30%;
        &:nth-child(3) {
          border-left: none ;
        }
      }
      @media screen and (max-width: 578px) {
        width: 50%;
        &:nth-child(2),&:nth-child(4) {
          border-left: none ;
        }
        &:nth-child(3) {
          border-left: 2px dashed rgba(189, 188, 188, 0.658);
        }
      }
    }
  }
}
</style>
