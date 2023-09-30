<template>
  <div class="wrap">
    <div class="content d-flex flex-column">
      <strong class="caption">دسترسی سریع</strong>
      <div class="socials mt-2">
        <div v-for="(item, index) in socials" :key="index" class="d-flex mt-2">
          <i class="icon-location-arrow"></i>
          <h6 class="mr-2">{{ item.title }}</h6>
        </div>
      </div>
    </div>
  </div>
</template>

  <script>
export default {
  name: 'QuickAccess',
  data() {
    return {
      socials: [
        { title: 'دانشنامه اتاق اصناف ایران' },
        { title: 'تالار گفتمان اتاق اصناف ایران' },
        { title: 'سامانه پست الکترونیک' },
        { title: 'سامانه مکاتبات سراسری' },
        { title: 'سامانه وب کنفرانس اتاق اصناف ایران' },
      ],
    }
  },
}
</script>

  <style scoped lang="scss">
.wrap {
  .content {
    .caption {
      font-size: 27px;
      text-align: right;
      font-family: 'B nazanin';
    }
    .socials {
      font-family: 'B nazanin';
      i{
        transform: rotate(220deg);
        font-size: 10px;
      }
      h6 {
        font-size: 12px;
        text-align: right;
        margin-bottom: 0;
      }
    }
  }
}
</style>
