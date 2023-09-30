<template>
  <div class="wrapper">
    <div class="wrap-menu">
      <ul class="d-flex justify-content-around h-75">
        <li v-for="(item, index) in items" :key="index">
          <div>
            <span> {{ item.title }} </span><i :class="item.icon"></i>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderMenu',
  data() {
    return {
      items: [
        { title: 'اخبار', icon: 'icon-keyboard_arrow_down' },
        { title: 'چندرسانه ای', icon: 'icon-keyboard_arrow_down' },
        { title: 'دسترسی سریع', icon: 'icon-keyboard_arrow_down' },
        { title: 'جستجوی پیشرفته' },
        { title: 'سامانه آموزش' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.wrapper {
  height: 100%;
  .wrap-menu {
    height: 100%;
    padding: 10px 0;
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
    border-radius: 13px;
    font-family: 'Traffic';
    @media screen and (max-width: 992px) {
      ul {
        flex-direction: column;
        align-items: center;
        i {
          display: none;
        }
      }
    }
    li {
      font-size: 18px;
      @media screen and (max-width: 992px) {
        width: 100%;
      }
      &:last-child {
        position: relative;
        &::before {
          @media screen and (max-width: 992px) {
            display: none;
          }
          position: absolute;
          content: '';
          bottom: -5px;
          left: 0%;
          width: 40%;
          height: 3px;
          background-color: white;
        }
      }
    }
  }
}
</style>
