<template>
  <div class="d-flex">
    <div
      class="right-section iran-logo d-flex flex-column align-items-center justify-content-center"
    >
      <img
        :src="require('@/assets/images/asnaf/iran-logo.png')"
        alt="iran-logo"
        width="50"
      />
      <p class="right-title text-center">اتاق اصناف ایران</p>
    </div>
    <HeaderMenu />
    <div
      class="left-section d-flex flex-column align-items-center justify-content-center"
    >
      <img
        :src="require('@/assets/images/asnaf/main-logo.png')"
        alt="main-logo"
        width="50"
      />
      <p class="left-title text-center">اتاق اصناف ایران</p>
    </div>
  </div>
</template>

<script>
import HeaderMenu from '@/components/asnaf/header/HeaderMenu.vue'
export default {
  name: 'HeaderTop',
  components: {
    HeaderMenu,
  },
}
</script>


<style scoped lang="scss">
.right-section,
.left-section {
  position: relative;
  width: 10%;
  margin-top: 15px;
  @media screen and (max-width: 768px) {
    width:15%
  }
  .right-title {
    color: #2d3191;
    font-size: 30px;
    font-weight: bold;
    font-family: 'IranNastaliq';
  }
  .left-title {
    color: #2d3191;
    font-size: 20px;
    font-weight: bold;
    font-family: 'IranNastaliq';
  }
}
</style>
