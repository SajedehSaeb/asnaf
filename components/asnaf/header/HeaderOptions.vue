<template>
  <div class="mt-3 wrap">
    <div class="single mt-2" v-for="(item, index) in items" :key="index">
      <p class="text-white">{{ item.title }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderOptions',
  data() {
    return {
      items: [
        { title: 'فراخوان بیمه تکمیلی گروهی درمان' },
        { title: 'فراخوان تجهیز اتاق اصناف ایران به سامانه مکاتبات اداری' },
        { title: 'روز ملی اصناف' },
        { title: 'گزارش عملکرداتاق اصناف ایران(1401-1397)' },
        { title: 'نمایشگاهی به وسعت ایران' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.wrap {
    width: 90%;
}
.single {
  background-color: #bf1e2e;
  text-align: center;
  border-radius: 15px;
  padding: 10px 5px;
}
</style>