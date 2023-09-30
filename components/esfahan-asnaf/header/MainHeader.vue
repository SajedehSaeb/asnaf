<template>
  <div class="main-header">
    <i class="icon-menu" @click="showMenu"></i>
    <div class="wrap-menu-option">
      <div class="menu-container">
        <i class="icon-x" @click="showMenu"></i>
        <ul class="d-flex flex-column justify-content-around mb-0 h-100">
          <li v-for="(item, index) in items" :key="index">
            <div>
              <span> {{ item.title }} </span>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="wrap-top">
      <div class="wrap-top-content">
        <div class="d-flex flex-column justify-content-between h-100">
          <div
            class="wrap-head d-flex justify-content-between align-items-center"
          >
            <h1 class="header-title">اتاق اصناف اصفهان</h1>
            <div
              class="header-logo d-flex flex-column align-items-center justify-content-center"
            >
              <img :src="require('@/assets/images/asnaf/main-logo.png')" />
              <h4 class="mt-1">اتاق اصناف اصفهان</h4>
            </div>
          </div>
        </div>
      </div>
      <div class="overlay"></div>
    </div>
    <div class="wrap-bottom pt-3">
      <img
        :src="require('@/assets/images/asnaf/tehran-asnaf/header-back.png')"
        class="back1"
      />
      <div class="w-60 mb-2">
        <HeaderMenu />
      </div>
      <div
        class="wrap-caption d-flex flex-column justify-content-center align-items-center w-60"
      >
        <img
          :src="require('@/assets/images/asnaf/tehran-asnaf/line.png')"
          class="w-100"
        />
      </div>
      <HeaderSocial />

      <b-row class="slider-head">
        <b-col cols="12" lg="9">
          <HeaderSlider />
        </b-col>
        <b-col cols="12" lg="3" class="slogan-wrapper">
          <div
            class="wrap-slogan d-flex flex-column justify-content-center align-items-center"
          >
            <img
              :src="require('@/assets/images/asnaf/tehran-asnaf/slogan.jpeg')"
            />
            <button class="mt-3">یادداشت</button>
          </div>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

  <script>
import HeaderMenu from '@/components/esfahan-asnaf/header/HeaderMenu.vue'
import HeaderSocial from '@/components/esfahan-asnaf/header/HeaderSocial.vue'
import HeaderSlider from '@/components/esfahan-asnaf/header/HeaderSlider.vue'
export default {
  name: 'MainHeader',
  components: { HeaderMenu, HeaderSocial, HeaderSlider },

  methods: {
    showMenu() {
      const iconMenu = document.querySelector('.icon-menu')
      const wrapMenu = document.querySelector('.wrap-menu-option')
      iconMenu.classList.toggle('extend-index')
      wrapMenu.classList.toggle('show-menu')
    },
  },
  data() {
    return {
      items: [
        { title: 'صفحه نخست' },
        { title: 'گالری عکس' },
        { title: 'ارسال مطلب و خبر' },
        { title: 'اطلاعات حقوقی' },
      ],
    }
  },
}
</script>

  <style scoped lang="scss">
.main-header {
  color: white;
  position: relative;
  .wrap-menu-option {
    display: none;
    .menu-container {
      height: 100%;
      position: relative;
      .icon-x {
        cursor: pointer;
        display: none;
        @media screen and (max-width: 1024px) {
          display: block !important;
          position: absolute;
          left: 3%;
          top: 5%;
          z-index: 1000;
        }
      }
    }
    @media screen and (max-width: 1024px) {
      display: block;
      transition: all 0.3s ease-in-out;
      text-align: right !important;
      position: absolute;
      right: 0;
      top: 0;
      width: 25%;
      height: 250px;
      z-index: 10000;
      border-radius: 15px 0 0 15px;
      transform: translateX(100%);
      opacity: 0;
      background-image: linear-gradient(
        270deg,
        hsl(182deg 97% 15%) 0%,
        hsl(182deg 96% 18%) 11%,
        hsl(182deg 95% 20%) 22%,
        hsl(182deg 94% 23%) 33%,
        hsl(182deg 93% 25%) 44%,
        hsl(182deg 91% 28%) 56%,
        hsl(182deg 90% 31%) 67%,
        hsl(182deg 89% 34%) 78%,
        hsl(182deg 87% 36%) 89%,
        hsl(182deg 86% 39%) 100%
      );
    }
    @media screen and (max-width: 768px) {
      width: 30%;
    }
    @media screen and (max-width: 578px) {
      width: 37%;
    }
    @media screen and (max-width: 450px) {
      width: 60%;
    }
  }
  .extend-index {
    z-index: -1 !important;
  }
  .show-menu {
    transform: translateX(0) !important;
    opacity: 1 !important;
    transition: all 0.3s ease-in-out;
  }
  .icon-menu {
    cursor: pointer;
    position: absolute;
    right: 5%;
    top: 2%;
    font-size: 35px;
    z-index: 5;
    display: none;
    @media screen and (max-width: 1024px) {
      display: block;
    }
  }
  .w-60 {
    width: 60%;
    margin: 0 auto;
  }
  .wrap-top {
    position: relative;
    background: url('../../../assets/images/asnaf/esfahan-asnaf/header.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: top;
    height: 410px;
    &-content {
      position: absolute;
      padding: 0 20px 0 20px;
      right: 0;
      left: 0;
      top: 0;
      bottom: 0;
      width: 100%;
      height: 100%;
      z-index: 3;
      .wrap-head {
        @media screen and (max-width: 578px) {
          flex-direction: column-reverse;
          height: 70%;
        }
        @media screen and (max-width: 1024px) {
          margin-top: 10px;
        }
        .header-logo {
          @media screen and (max-width: 578px) {
            width: 100%;
            align-items: flex-end !important;
          }
          img {
            width: 80px;
          }
          h4 {
            font-size: 50px;
            font-family: 'IranNastaliq';
            @media screen and (max-width: 768px) {
              font-size: 16px !important;
            }
          }
        }
        .header-title {
          font-family: 'IranNastaliq';
          text-shadow: 4px 4px 2px rgba(0, 0, 0, 0.6);
          font-size: 120px;
          margin-right: 140px;
          margin-top: 100px;
          @media screen and (max-width: 578px) {
            margin-right: 0;
          }
          @media screen and (max-width: 768px) {
            font-size: 30px !important;
          }
          @media screen and (max-width: 1024px) {
            font-size: 40px;
            margin-top: 0px;
          }
        }
      }
    }

    .overlay {
      position: absolute;
      right: 0;
      left: 0;
      top: 0;
      bottom: 0;
      width: 100%;
      height: 100%;
      background: rgba(21, 236, 243, 0.61);
      z-index: 2;
    }
  }
  .wrap-bottom {
    border-top: 1px solid white;
    position: relative;
    padding-bottom: 60px;
    background-image: linear-gradient(
      270deg,
      hsl(182deg 97% 15%) 0%,
      hsl(182deg 96% 18%) 11%,
      hsl(182deg 95% 20%) 22%,
      hsl(182deg 94% 23%) 33%,
      hsl(182deg 93% 25%) 44%,
      hsl(182deg 91% 28%) 56%,
      hsl(182deg 90% 31%) 67%,
      hsl(182deg 89% 34%) 78%,
      hsl(182deg 87% 36%) 89%,
      hsl(182deg 86% 39%) 100%
    );
    .wrap-socials {
      position: absolute;
      left: 7%;
      top: 0;
      @media screen and (max-width: 1024px) {
        width: 100%;
        left: 0;
      }
    }

    .back1 {
      position: absolute;
      bottom: 1%;
      left: 10%;
    }

    .slider-head {
      width: 70%;
      margin: 0 auto;
      margin-top: 60px;
      .slogan-wrapper {
        @media screen and (max-width: 1024px) {
          margin-top: 35px;
        }
      }
      .wrap-slogan {
        img {
          border-radius: 40px;
          width: 100%;
          border: 2px solid white;
          border-radius: 40px;
        }
        button {
          height: 30%;
          color: white;
          font-weight: bolder;
          background-image: linear-gradient(
            270deg,
            hsl(182deg 97% 15%) 0%,
            hsl(182deg 96% 18%) 11%,
            hsl(182deg 95% 20%) 22%,
            hsl(182deg 94% 23%) 33%,
            hsl(182deg 93% 25%) 44%,
            hsl(182deg 91% 28%) 56%,
            hsl(182deg 90% 31%) 67%,
            hsl(182deg 89% 34%) 78%,
            hsl(182deg 87% 36%) 89%,
            hsl(182deg 86% 39%) 100%
          );
          border: none;
          -webkit-box-shadow: 6px 6px 12px -1px rgba(0, 0, 0, 0.63);
          -moz-box-shadow: 6px 6px 12px -1px rgba(0, 0, 0, 0.63);
          box-shadow: 6px 6px 12px -1px rgba(0, 0, 0, 0.63);
          width: 80%;
          height: 60px;
          border-radius: 15px;
          font-size:30px;
          font-family: 'B nazanin';
        }
      }
    }
  }
}
</style>
