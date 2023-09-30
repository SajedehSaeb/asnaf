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
    90deg,
    hsl(287, 16%, 51%) 0%,
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
  .options {
    background-color: #6d6e70;
    padding: 10px 0 30px 0;
    color: white;
    font-family: 'Traffic';
    li {
      border-left: 1px solid #00b0b7;
      font-size: 15px;
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
