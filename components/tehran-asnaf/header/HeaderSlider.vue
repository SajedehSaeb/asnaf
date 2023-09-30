<template>
  <div class="wrap">
    <div class="content"></div>
    <div class="wrap-slider mt-3">
      <swiper
        ref="mySwiper"
        :options="swiperOptions"
        @slideChangeTransitionStart="handleSlideChange"
      >
        <template>
          <swiper-slide v-for="item in 10" :key="item.id">
            <div class="wrap-img">
              <img :src="require('@/assets/images/asnaf/room.jpg')" />
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
  name: 'TehranHeaderSlider',
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

  methods: {
    handleSlideChange() {
      const swiper = this.$refs.mySwiper.$swiper
      this.activeIndex = swiper.activeIndex
      const next = breakpoints[swiper.currentBreakpoint]
      this.lastIndex = Math.max(this.$refs.mySwiper.$children.length - next, 0)
    },

    nextSlide(val) {
      const swiper = this.$refs.mySwiper.$swiper
      const next = breakpoints[swiper.currentBreakpoint]
      if (val === 'next') {
        swiper.slideTo(swiper.activeIndex + next)
      } else {
        swiper.slideTo(swiper.activeIndex - next)
      }
    },
  },
}
</script>
    
    <style scoped lang="scss" >
.wrap {
  position: relative;
  .content {
    position: absolute;
    width: 100%;
    height: 100%;
    left: 5%;
    bottom: -5%;
    border: 2px solid white;
    border-radius: 25px;
  }
  &-slider {
    .swiper-container {
      border-radius: 25px;
      .swiper-wrapper {
        .swiper-slide {
          border-radius: 25px;
          .wrap-img {
            height: 500px;
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
.single_btn {
  width: 15px !important;
  height: 35px !important;
}
</style>
    