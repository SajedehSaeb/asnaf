<template>
  <div class="wrap-header">
    <img
      :src="require('@/assets/images/asnaf/header-back1.png')"
      class="back1"
    />
    <img
      :src="require('@/assets/images/asnaf/header-back2.png')"
      class="back2"
    />
    <i class="icon-menu" @click="showMenu"></i>
    <HeaderTop />
    <HeaderBottom />
  </div>
</template>

<script>
import HeaderTop from '@/components/asnaf/header/HeaderTop.vue'
import HeaderBottom from '@/components/asnaf/header/HeaderBottom.vue'
export default {
  name: 'HeaderComponent',
  components: {
    HeaderTop,
    HeaderBottom,
  },
  methods: {
    showMenu() {
      // const iconMenu = document.querySelector('.icon-menu')
      const wrapMenu = document.querySelector('.menus-options')
      console.log(wrapMenu,"wrapMenu")
      // iconMenu.classList.toggle('extend-index')
       wrapMenu.classList.toggle('show-menu')
    },
  },
}
</script>

<style scoped lang="scss">
.wrap-header {
  background-image: linear-gradient(
    270deg,
    hsl(201deg 64% 91%) 0%,
    hsl(202deg 60% 89%) 13%,
    hsl(203deg 57% 88%) 23%,
    hsl(203deg 54% 86%) 33%,
    hsl(204deg 52% 84%) 43%,
    hsl(205deg 51% 83%) 52%,
    hsl(209deg 48% 81%) 62%,
    hsl(212deg 45% 79%) 71%,
    hsl(217deg 41% 78%) 81%,
    hsl(222deg 37% 76%) 90%,
    hsl(229deg 33% 75%) 100%
  );
  padding: 0 15px 25px 15px;
  min-height: 100vh;
  position: relative;
  .back1 {
    position: absolute;
    bottom: 0;
    left: 0;
    opacity: .5;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
  .back2 {
    position: absolute;
    top: 0;
    right: 0;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
  .icon-menu{
    cursor: pointer;
    display: none;
    position: absolute;
    left: 13%;
    top: 3%;
    z-index: 100;
    font-size: 35px;
    color: #283891;
    @media screen and (max-width:1200px) {
      display: block;
    }
    @media screen and (max-width:768px) {
      left: 25%;
    }
  }
}
</style>