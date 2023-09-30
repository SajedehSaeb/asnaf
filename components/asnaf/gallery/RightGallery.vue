<template>
  <div class="wrap w-100">
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
    <div class="images d-flex justify-content-between mt-2">
      <img v-for="(item,index) in 3" :key="index" :src="require('@/assets/images/asnaf/room.jpg')" />
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
  name: 'RightGallery',
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
  &-slider {
    border-radius: 25px;
    .swiper-container {
      border-radius: 25px;
      .swiper-wrapper {
        .swiper-slide {
          border: 1px solid white;
          border-radius: 25px;
          .wrap-img {
            height: 300px;
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
  .images{
    width: 90%;
    margin: 0 auto;
    img{
      width: 30%;
      border-radius: 20px;
      border: 1px solid white;
    }
  }
}
.single_btn {
  width: 15px !important;
  height: 35px !important;
}
</style>
  