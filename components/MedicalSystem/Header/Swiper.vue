<template>
  <div class="image-medical">
    <div class="background">
      <div class="background1">
        <div class="imge">
          <img :src="require('@/assets/medical/salamat.jpg')" class="w-100 h-100 imge-salamat"/>
        </div>
      </div>
    </div>
    <div class="white-border"></div>
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
  name: 'RightHeaderSlider',
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

<style scoped>
.background {
  background-color: #662d91;
  height: 70vh;
  width: 85vw;
  z-index: 1;
  border-radius: 50px;
  position: absolute;
  top: 12%;
  left: 7%;
}

.background1 {
  height: 70vh;
  width: 85vw;
  border-radius: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.imge{
  width: 85%;
  height: 75%;
  border-radius: 50px;
  /* background-image: url('@/assets/medical/salamat.jpg'); */
  /* background-repeat: no-repeat; */
}

.imge-salamat{
  border-radius: 50px;
}

.white-border {
  border: 1px solid white;
  height: 70vh;
  width: 85vw;
  position: absolute;
  top: 11%;
  left: 10%;
  border-radius: 60px;
}

.image-medical {
  z-index: 1;
}
</style>
