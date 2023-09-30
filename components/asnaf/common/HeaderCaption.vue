<template>
  <div class="wrap w-100">
    <div class="wrap-line">
      <img
        :src="require('@/assets/images/asnaf/news/line3.png')"
        alt="news"
        class="w-100"
      />
      <span class="title text-white">{{ title }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderCaption',
  props: {
    title: {
      default: '',
      type: String,
    },
  },
}
</script>

<style scoped lang="scss">
.wrap {
  &-line {
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    .title {
      text-align: center;
      position: absolute;
      background-color: #283891;
      top: 30%;
      padding: 17px 40px;
      font-size: 25px;
      border-radius: 0 0 25px 25px;
      display: flex;
      justify-content: center;
      align-items: center;
      @media screen and (max-width: 768px) {
        font-size: 18px;
      }
    }
  }
}
</style>