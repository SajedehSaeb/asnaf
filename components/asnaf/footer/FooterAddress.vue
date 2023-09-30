<template>
  <div class="wrap">
    <div class="content d-flex flex-column">
      <strong class="caption">نشانی</strong>
      <div class="socials mt-2">
        <div v-for="(item, index) in socials" :key="index" class="d-flex">
          <h6 class="mr-2">{{ item.title }}</h6>
        </div>
      </div>
    </div>
  </div>
</template>

    <script>
export default {
  name: 'FooterAddress',
  data() {
    return {
      socials: [
        {
          title:
            'تهرانی , خیابان قائم مقام فراهانی , میدان شعاع , ابتدای خیابان گلریز , نبش کوچه وفا , پلاک 1',
        },
        { title: 'کد پستی' },
        { title: '1589633111' },
        { title: 'تلفن' },
        { title: '88345962' },
        { title: '88345962' }
      ],
    }
  },
}
</script>

    <style scoped lang="scss">
.wrap {
  .content {
    .caption {
      font-family: 'B nazanin';
      font-size: 27px;
      text-align: right;
    }
    .socials {
      font-family: 'B nazanin';
      h6 {
        font-size: 12px;
        text-align: right;
        line-height: 2;
      }
    }
  }
}
</style>
