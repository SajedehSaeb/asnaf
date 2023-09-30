<template>
  <div class="menus">
    <ul class="menus-options d-flex justify-content-around">
      <li v-for="(item, index) in items" :key="index">
        {{ item.caption }}
        <i :class="item.icon"></i>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HeaderMenu',
  data() {
    return {
      items: [
        { caption: 'صفحه اصلی' },
        { caption: 'اتاق اصناف ایران', icon: 'icon-keyboard_arrow_down' },
        { caption: 'کمیسیون ها', icon: 'icon-keyboard_arrow_down' },
        { caption: 'اتحادیه های کشوری', icon: 'icon-keyboard_arrow_down' },
        { caption: 'قوانین و مقررات', icon: 'icon-keyboard_arrow_down' },
        { caption: 'کرونا', icon: 'icon-keyboard_arrow_down' },
        { caption: 'آموزش', icon: 'icon-keyboard_arrow_down' },
        { caption: 'رویدادها', icon: 'icon-keyboard_arrow_down' },
        { caption: 'درباره ما' },
        { caption: 'تماس با ما' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.menus {
  text-align: right;
  width: 80%;
  color: #2d3191;
  background-image: linear-gradient(
    270deg,
    hsl(202deg 65% 91%) 0%,
    hsl(203deg 59% 87%) 12%,
    hsl(204deg 55% 84%) 21%,
    hsl(205deg 53% 80%) 30%,
    hsl(206deg 51% 76%) 39%,
    hsl(208deg 49% 72%) 48%,
    hsl(210deg 46% 68%) 57%,
    hsl(212deg 44% 64%) 65%,
    hsl(215deg 42% 62%) 74%,
    hsl(219deg 39% 61%) 82%,
    hsl(224deg 36% 60%) 91%,
    hsl(231deg 32% 59%) 100%
  );
  display: flex;
  justify-content: center;
  align-items: end;
  border-radius: 0 0 20px 20px;
  font-family: 'B nazanin';
  @media screen and (max-width: 768px) {
    width: 70%;
  }
  .show-menu {
    transform: translateX(0) !important;
    opacity: 1 !important;
    transition: all 0.3s ease-in-out;
  }
  &-options {
    width: 100%;
    @media screen and (max-width: 1200px) {
      position: absolute;
      right: 0;
      top: 0;
      width: 25%;
      background-color: #283891;
      color: white;
      height: 50%;
      flex-direction: column;
      z-index: 2;
      border-radius: 15px 0 0 15px;
      font-weight: bold;
      transform: translateX(100%);
      opacity: 0;
      transition: all 0.3s ease-in-out;
    }
    @media screen and (max-width: 992px) {
      width: 30%;
      height: 30%;
    }
    @media screen and (max-width: 768px) {
      width: 40%;
      height: 30%;
    }
    @media screen and (max-width: 578px) {
      width: 65%;
      height: 30%;
    }
  }
}
</style>
