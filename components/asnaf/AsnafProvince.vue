<template>
  <div class="content">
    <img
      :src="require('@/assets/images/asnaf/province-back.png')"
      class="back"
    />
    <div class="wrap mt-3">
      <div class="head">
        <HeaderCaption title="اتاق اصناف استان ها" />
      </div>
      <div class="map d-flex justify-content-center align-items-center">
        <img :src="require('@/assets/images/asnaf/map.png')"/>
      </div>
      <div class="d-flex justify-content-center align-items-center my-4">
        <b-button
          class="arshive px-3 py-2 d-flex justify-content-center align-items-center"
        >
          <span>اطلاعات بیشتر</span>
          <div class="wrap-arrow mt-1">
            <i class="icon-keyboard_arrow_left"></i
            ><i class="icon-keyboard_arrow_left second"></i>
          </div>
        </b-button>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderCaption from '~/components/asnaf/common/HeaderCaption.vue'
export default {
  name: 'AsnafProvince',
  components: { HeaderCaption },
}
</script>

<style scoped lang="scss">
.content {
  position: relative;
  .back {
    position: absolute;
    right: 0;
    top: -20%;
    @media screen and (max-width: 578px) {
      display: none;
    }
  }
  .wrap {
    width: 70%;
    margin: 0 auto;
    position: relative;
    .map {

      img {
        width: 100%;
        height: 100%;
        margin-top: 1rem;
        @media screen and (max-width: 578px) {
          margin-top:90px;
        }
      }
    }
    .head {
      position: absolute;
      right: 0;
      left: 0;
      font-family: 'B nazanin';
    }
    .arshive {
      background-color: #9e1f63;
      border: none;
      border-radius: 8px;
      font-size: 12px;
      .wrap-arrow {
        position: relative;
        .second {
          position: absolute;
          left: -50%;
          top: 17%;
        }
      }
    }
  }
}
</style>
