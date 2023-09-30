<template>
  <div >
    <GoldSellersLine />
    <div class="navbar-header" dir="rtl">
      <b-navbar toggleable="lg" type="dark" class="navbar-background">
        <!-- <b-navbar-brand href="#"></b-navbar-brand> -->

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item href="#">صفحه اصلی</b-nav-item>
            <b-nav-item href="#">گالری تصاویر</b-nav-item>
            <b-nav-item href="#">نرخ های مرجع</b-nav-item>
            <b-nav-item href="#">اطلاعیه و بخشنامه</b-nav-item>
            <b-nav-item href="#">مدارک</b-nav-item>
            <b-nav-item href="#">واحدهای صنفی</b-nav-item>
            <b-nav-item href="#">پرداخت حق عضویت</b-nav-item>
            <b-nav-item href="#">فیلم</b-nav-item>
            <b-nav-item href="#">آموزش</b-nav-item>
            <b-nav-item href="#">کد های باطله</b-nav-item>
          </b-navbar-nav>

        </b-collapse>
      </b-navbar>
    </div>
    <div class="d-flex justify-content-center align-item-center ">
      <div
        class=" w-75 px-2 py-1 d-flex justify-content-start align-item-end "
      >
        <GoldSellersHeaderSocialMedia />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.navbar-background {
  background: linear-gradient(
    305deg,
    rgb(178, 127, 43, 50%),
    rgb(247, 222, 124, 50%),
    rgb(178, 127, 43, 50%),
    rgb(247, 222, 124, 50%),
    rgb(178, 127, 43, 50%)
  );
  /* opacity: 50%; */

  width: 75%;
  border-radius: 10px;
}

.navbar-header {
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: 'Traffic';
  font-size: 20px;
}

.navbar-dark .navbar-nav .nav-link {
  color: #231f20;
  text-align: end;
}

@media (width: 1024px) {
  .navbar-dark .navbar-nav .nav-link {
    font-size: 12px;
}
}
</style>
