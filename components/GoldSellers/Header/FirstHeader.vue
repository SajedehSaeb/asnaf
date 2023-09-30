<template>
  <div class="header">
    <GoldSellersHeaderNavBar />
    <div class="diamond d-none d-lg-flex">
      <b-img src="@/assets/goldSeller/Asset 21.png" />
    </div>
    <div class="circle d-none d-lg-flex">
      <GoldSellersHeaderCircle />
    </div>

    <div class="w-100 d-flex justify-content-center align-item-center">
      <b-row class="w-100 mt-3 p-4">
        <b-col cols="12" md="8" lg="7" xl="3"></b-col>
        <b-col cols="12" md="8" lg="7" xl="7">
          <GoldSellersHeaderMovieComponent />
        </b-col>
        <b-col cols="12" md="4" lg="3" xl="2">
          <GoldSellersHeaderNews />
        </b-col>

      </b-row>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.header {
  background-image: linear-gradient(#ffffff, rgb(229, 201, 161, 50%));
  position: relative;
  /* height: 88vh; */
}

@media (max-width: 768px) {
  /* .header {
    height: 160vh;
  } */
}

.diamond {
  position: absolute;
  bottom: 0;
  right: 2%;
}

.circle {
  position: absolute;
  bottom: 35%;
  right: 18%;
}
</style>
