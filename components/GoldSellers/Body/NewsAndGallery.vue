<template>
  <div class="background">
    <div class="diamond">
      <b-img src="@/assets/goldSeller/Asset 20.png" />
    </div>
    <div class="diamond-bottom">
      <b-img src="@/assets/goldSeller/Asset 28.png" />
    </div>
    <div class="diamond-middle">
      <b-img src="@/assets/goldSeller/Asset 27.png" />
    </div>
    <div class="diamond-middle2">
      <b-img src="@/assets/goldSeller/Asset 26.png" />
    </div>
    <div class="diamond-bottom1">
      <b-img src="@/assets/goldSeller/Asset 29.png" />
    </div>
    <GoldSellersLine />
    <GoldSellersBodyLastNews />
    <GoldSellersBodyGallery />
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.background {
  background-image: linear-gradient(#ffffff, rgb(229, 201, 161, 50%));
  /* height: 150vh; */
  position: relative;
}

.diamond {
  position: absolute;
  top: 0;
  right: 3%;
}

.diamond-bottom {
  position: absolute;
  bottom: 0;
  left: 3%;
}

.diamond-bottom1 {
  position: absolute;
  bottom: 0;
  right: 3%;
}

.diamond-middle {
  position: absolute;
  top:40%;
  left: 3%;
}

.diamond-middle2 {
  position: absolute;
  top: 55%;
  right: 8%;
}
</style>
