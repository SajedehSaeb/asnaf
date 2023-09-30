<template>
  <div class="wrapper">
    <div class="wrap-menu">
      <ul class="d-flex justify-content-around h-75 mb-0">
        <li v-for="(item, index) in items" :key="index">
          <div>
            <span> {{ item.title }} </span>
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
        { title: 'صفحه نخست' },
        { title: 'گالری عکس' },
        { title: 'ارسال مطلب و خبر' },
        { title: 'اطلاعات حقوقی' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.wrapper {
  width: 75%;
  margin: 0 auto;
  height: 100%;
  @media screen and (max-width: 1200px) {
     margin-top: 55px;
     width: 90%;
    }
  @media screen and (max-width: 1024px) {
    display: none;
    }
  .wrap-menu {
    font-family: 'Traffic';
    height: 100%;
    padding: 10px 0;
    background-color: white;
    color: #00a79d;
    border-radius: 20px;
    @media screen and (max-width: 1024px) {
      ul {
        flex-direction: column;
        align-items: center;
      }
    }
    li {
      font-size: 18px;
      @media screen and (max-width: 1024px) {
        width: 100%;
      }
    }
  }
}
</style>
