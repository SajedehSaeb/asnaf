<template>
  <div class="main-header">
    <i class="icon-menu" @click="showMenu"></i>
    <div class="wrap-top">
      <div class="wrap-top-content">
        <div class="d-flex flex-column justify-content-between h-100">
          <div
            class="wrap-head d-flex justify-content-between align-items-center"
          >
            <h1 class="header-title">اتاق اصناف تهران</h1>
            <div
              class="header-logo d-flex flex-column align-items-center justify-content-center"
            >
              <img :src="require('@/assets/images/asnaf/main-logo.png')" />
              <h4 class="mt-1">اتاق اصناف تهران</h4>
            </div>
          </div>
          <div class="wrap-menu-option w-60">
            <div class="menu-container">
              <i class="icon-x" @click="showMenu"></i>
              <HeaderMenu />
            </div>
          </div>
        </div>
      </div>
      <div class="overlay"></div>
    </div>
    <div class="wrap-bottom">
      <img
        :src="require('@/assets/images/asnaf/tehran-asnaf/header-back.png')"
        class="back1"
      />
      <div
        class="wrap-caption d-flex flex-column justify-content-center align-items-center w-60"
      >
        <img
          :src="require('@/assets/images/asnaf/tehran-asnaf/line.png')"
          class="w-100"
        />
        <HeaderSocial />
      </div>
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
import HeaderMenu from '@/components/tehran-asnaf/header/HeaderMenu.vue'
import HeaderSocial from '@/components/tehran-asnaf/header/HeaderSocial.vue'
import HeaderSlider from '@/components/tehran-asnaf/header/HeaderSlider.vue'
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
}
</script>

  <style scoped lang="scss">
.main-header {
  color: white;
  position: relative;
  .extend-index {
    z-index: -1 !important;
  }
  .icon-menu {
    cursor: pointer;
    position: absolute;
    right: 5%;
    top: 2%;
    font-size: 35px;
    z-index: 5;
    display: none;
    @media screen and (max-width: 992px) {
      display: block;
    }
  }
  .w-60 {
    width: 60%;
    margin: 0 auto;
  }
  .wrap-top {
    position: relative;
    background: url('../../../assets/images/asnaf/tehran-asnaf/header.jpg');
    background-size: cover;
    height: 290px;
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
      .show-menu {
        transform: translateX(0) !important;
        opacity: 1 !important;
        transition: all 0.3s ease-in-out;
      }
      .wrap-menu-option {
        .menu-container {
          height: 100%;
          position: relative;
          .icon-x {
            cursor: pointer;
            display: none;
            @media screen and (max-width: 992px) {
              display: block !important;
              position: absolute;
              left: 3%;
              top: 5%;
              z-index: 1000;
            }
          }
        }
        @media screen and (max-width: 992px) {
          transition: all 0.3s ease-in-out;
          text-align: right !important;
          position: absolute;
          right: 0;
          bottom: 0;
          width: 25%;
          height: 100%;
          z-index: 10000;
          border-radius: 15px 0 0 15px;
          transform: translateX(100%);
          opacity: 0;
          background-image: linear-gradient(
            90deg,
            hsl(238deg 28% 65%) 0%,
            hsl(238deg 26% 62%) 11%,
            hsl(238deg 23% 59%) 22%,
            hsl(238deg 21% 57%) 33%,
            hsl(237deg 20% 54%) 44%,
            hsl(237deg 18% 51%) 56%,
            hsl(237deg 17% 49%) 67%,
            hsl(237deg 18% 46%) 78%,
            hsl(237deg 18% 44%) 89%,
            hsl(237deg 19% 41%) 100%
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
      .wrap-head {
        @media screen and (max-width: 578px) {
          flex-direction: column-reverse;
          height: 70%;
        }
        @media screen and (max-width: 992px) {
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
            font-size: 30px;
            font-family: 'IranNastaliq';
            @media screen and (max-width: 768px) {
              font-size: 16px !important;

            }
          }
        }
        .header-title {
          font-family: 'IranNastaliq';
          text-shadow: 2px 5px 4px black;
          font-size: 120px;
          margin-right: 140px;
          margin-top: 50px;
          @media screen and (max-width: 578px) {
            margin-right: 0;
          }
          @media screen and (max-width: 768px) {
            font-size: 30px !important;
          }
          @media screen and (max-width: 992px) {
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
      background: rgba(117, 113, 117, 0.521);
      z-index: 2;
    }
  }
  .wrap-bottom {
    position: relative;
    padding-bottom: 60px;
    background-image: linear-gradient(
      90deg,
      hsl(285deg 18% 43%) 0%,
      hsl(285deg 19% 41%) 11%,
      hsl(285deg 20% 39%) 22%,
      hsl(285deg 22% 37%) 33%,
      hsl(285deg 23% 35%) 44%,
      hsl(285deg 24% 33%) 56%,
      hsl(285deg 26% 31%) 67%,
      hsl(285deg 28% 29%) 78%,
      hsl(285deg 30% 27%) 89%,
      hsl(285deg 32% 25%) 100%
    );
    .back1 {
      position: absolute;
      bottom: 1%;
      left: 10%;
    }
    .wrap-caption {
      position: relative;
      .wrap-socials {
        position: absolute;
        content: '';
        top: 5px;
      }
    }
    .slider-head {
      width: 70%;
      margin: 0 auto;
      margin-top: 60px;
      .slogan-wrapper {
        @media screen and (max-width: 992px) {
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
            90deg,
            hsl(238deg 28% 65%) 0%,
            hsl(238deg 26% 62%) 11%,
            hsl(238deg 23% 59%) 22%,
            hsl(238deg 21% 57%) 33%,
            hsl(237deg 20% 54%) 44%,
            hsl(237deg 18% 51%) 56%,
            hsl(237deg 17% 49%) 67%,
            hsl(237deg 18% 46%) 78%,
            hsl(237deg 18% 44%) 89%,
            hsl(237deg 19% 41%) 100%
          );
          border: none;
          -webkit-box-shadow: 6px 6px 12px -1px rgba(0, 0, 0, 0.63);
          -moz-box-shadow: 6px 6px 12px -1px rgba(0, 0, 0, 0.63);
          box-shadow: 6px 6px 12px -1px rgba(0, 0, 0, 0.63);
          width: 80%;
          height: 60px;
          border-radius: 15px;
          font-size: 20px;
        }
      }
    }
  }
}
</style>
