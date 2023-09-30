<template>
  <div class="wrap mt-15">
    <div class="content">
      <div class="d-flex justify-content-center align-center">
        <h4 class="text-white">یادداشت روز</h4>
      </div>
    </div>
    <div class="wrap-slider mt-3">
      <swiper ref="mySwiper" :options="swiperOptions">
        <template>
          <swiper-slide v-for="item in 10" :key="item.id">
            <div class="wrap-img">
              <img :src="require('@/assets/images/asnaf/dayNote.jpg')" />
            </div>
          </swiper-slide>
        </template>
      </swiper>
    </div>
  </div>
</template>
    
    <script>
import { Swiper, SwiperSlide } from 'vue-awesome-swiper'
import SwiperCore, { Pagination, Autoplay } from 'swiper/core'
import 'swiper/swiper-bundle.min.css'
import 'swiper/swiper.min.css'
SwiperCore.use([Pagination, Autoplay])
const breakpoints = {
  1904: 1,
  1024: 1,
  768: 1,
  640: 1,
}
export default {
  name: 'LeftHeaderSlider',
  components: {
    Swiper,
    SwiperSlide,
  },

  data() {
    return {
      swiperOptions: {
        autoplay: {
          delay: 1500,
          disableOnInteraction: false,
        },
        pagination: {
          el: '.swiper-pagination',
          clickable: true,
        },
        spaceBetween: 10,
        breakpoints: {
          1904: {
            slidesPerView: breakpoints['1904'],
            spaceBetween: 10,
          },
          1024: {
            slidesPerView: breakpoints['1024'],
            spaceBetween: 10,
          },
          768: {
            slidesPerView: breakpoints['768'],
            spaceBetween: 10,
          },
          640: {
            slidesPerView: breakpoints['640'],
            spaceBetween: 10,
          },
        },
      },
    }
  },
}
</script>
    
    <style scoped lang="scss" >
.wrap {
  position: relative;
  @media screen and (max-width:992px) {
    margin-top: 50px;
  }
  .content {
    position: absolute;
    z-index: 100;
    width: 100%;
    height: 100%;
    left: 5%;
    top: 2%;
    border: 2px solid #283891;
    border-radius: 25px;
  }
  &-slider {
    background-color: #283891;
    padding: 70px 25px 60px 25px;
    border-radius: 25px;
    .swiper-container {
      border-radius: 25px;
      .swiper-wrapper {
        .swiper-slide {
          border: 3px solid white;
          border-radius: 25px;
          .wrap-img {
            height: 400px;
            border-radius: 25px;
            img {
              width: 100%;
              height: 100%;
              border-radius: 25px;
            }
          }
        }
      }
    }
  }
}
</style>
    