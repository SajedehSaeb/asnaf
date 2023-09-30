<template>
  <div class="header-style position-relative">

    <div class="w-100 d-flex justify-content-center align-items-center">
      <MedicalSystemHeaderSocialMedia />
    </div>
    <div class="swiper-component">
      <MedicalSystemHeaderSwiper />
    </div>
    <div class="w-100 d-none d-md-flex justify-content-center align-items-center ">
      <MedicalSystemHeaderOtherNavbar />
    </div>

    <div class="img1">
      <b-img src="@/assets/medical/Asset 11.png" />
    </div>
    <div class="img2 d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 12.png" />
    </div>
    <div class="img3">
      <b-img src="@/assets/medical/Asset 14.png" />
    </div>
    <div class="img4">
      <b-img src="@/assets/medical/Asset 14.png" />
    </div>
    <div class="img5">
      <b-img src="@/assets/medical/Asset 18.png" />
    </div>
    <div class="img6 d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 12.png" />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.header-style {
  background-image: linear-gradient(
    130deg,
    rgb(140, 76, 143, 45%),
    rgb(140, 76, 143, 30%),
    rgb(93, 173, 209, 20%)
  );
  height: 100vh;
}

.swiper-component {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh;
}

.img1 {
  position: absolute;
  bottom: 0;
  left: 0;
}

.img2 {
  position: absolute;
  bottom: 2%;
  right: 8%;
}

.img3 {
  position: absolute;
  bottom: 8%;
  right: 6%;
}

.img4 {
  position: absolute;
  top: 6%;
  left: 2%;
}

.img5 {
  position: absolute;
  top: 7%;
  left: 4%;
}

.img6 {
  position: absolute;
  top: -0.5%;
  left: 11%;
}
</style>
