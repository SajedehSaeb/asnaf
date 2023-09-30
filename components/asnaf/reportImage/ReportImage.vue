<template>
  <div class="wrap-report">
    <img
      :src="require('@/assets/images/asnaf/report/report-back.png')"
      class="back-report"
    />
    <div class="wrap">
      <HeaderCaption title="گزارش تصویری" />
      <b-row class="reports mb-4">
        <b-col
          class="wrap-card px-0"
          v-for="(item, index) in 3"
          :key="index"
          cols="12"
          lg="3"
          md="8"
        >
          <div class="back-line"></div>
          <div class="wrap-img">
            <img :src="require(`@/assets/images/asnaf/report/1.png`)" />
          </div>
        </b-col>
      </b-row>
      <div class="d-flex justify-content-center align-items-center mt-5 mb-4">
        <b-button
          class="arshive px-3 py-2 d-flex justify-content-center align-items-center"
        >
          <span>آرشیو</span>
          <div class="wrap-arrow mt-1">
            <i class="icon-keyboard_arrow_left"></i
            ><i class="icon-keyboard_arrow_left second"></i></div
        ></b-button>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderCaption from '~/components/asnaf/common/HeaderCaption.vue'
export default {
  name: 'ReportImage',
  components: { HeaderCaption },
}
</script>

<style scoped lang="scss">
.wrap-report {
  position: relative;
  .back-report {
    position: absolute;
    right: 0;
    bottom: 0;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
  .wrap {
    width: 70%;
    margin: 0 auto;
    font-family: 'B nazanin';

    .reports {
      margin-top: 100px;
      justify-content: space-between;
      @media screen and (max-width: 992px) {
        justify-content: center;
      }
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
          top: 20%;
        }
      }
    }
    &-card {
      position: relative;
      @media screen and (max-width: 992px) {
        margin-top: 50px;
      }
      .back-line {
        position: absolute;
        z-index: -1;
        width: 100%;
        height: 100%;
        left: -12%;
        top: 7%;
        border: 1px solid #2b3990;
        border-radius: 30px;
      }
      .wrap-img {
        background-color: #2b3990;
        border-radius: 30px;
        width: 100%;
        height: 280px;
        padding: 15px;
        img {
          width: 100%;
          height: 100%;
          border-radius: 30px;
          border: 2px solid white;
        }
      }
    }
  }
}
</style>
