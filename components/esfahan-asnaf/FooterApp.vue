<template>
  <footer class="wrap">
    <ul class="options d-flex justify-content-center mb-0">
      <li v-for="(item, index) in options" :key="index" class="px-3">
        {{ item.title }}
      </li>
    </ul>
    <div class="footer-bottom">
      <div
        class="socials d-flex justify-content-center align-items-center px-2 py-3"
      >
        <div>
          <i
            v-for="(icon, index) in socials"
            :key="index"
            :class="icon.title"
            class="mx-2"
          ></i>
        </div>
        <img
          class="mx-2"
          :src="require('@/assets/images/asnaf/tehran-asnaf/eta.png')"
        />
        <i class="icon-house mx-2"></i>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterApp',
  data() {
    return {
      socials: [
        {
          title: 'icon-twitter',
        },
        { title: 'icon-facebook' },
        { title: 'icon-instagram' },
        {
          title: 'icon-youtube',
        },
      ],
      options: [
        { title: 'صفحه اصلی' },
        { title: 'درباره ما' },
        { title: 'تماس' },
        { title: 'با ما' },
        { title: 'قوانین و مقررات' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.wrap {
  padding-top: 10px;
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
  .options {
    background-color: #6d6e70;
    padding: 10px 0 30px 0;
    color: white;
    li {
      border-left: 1px solid #00b0b7;
      font-size: 15px;
      font-family: 'Traffic';
      @media screen and (max-width: 578px) {
        font-size: 13px;
        padding: 0 5px !important;
      }
      &:last-child {
        border-left: none !important;
      }
    }
  }
  .footer-bottom {
    background-color: #808285;
    height: 130px;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    .socials {
      position: absolute;
      top: 1px;
      z-index: 1000;
      background-color: #6d6e70;
      color: white;
      font-size: 20px;
      border-radius: 15px;
      -webkit-box-shadow: 4px 4px 7px 5px rgba(77, 75, 77, 1);
      -moz-box-shadow: 4px 4px 7px 5px rgba(77, 75, 77, 1);
      box-shadow: 4px 4px 7px 5px rgba(77, 75, 77, 1);
    }
  }
}
</style>
