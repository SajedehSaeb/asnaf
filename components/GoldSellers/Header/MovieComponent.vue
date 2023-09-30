<template>
  <div class="movie-border mt-2">
    <div class="border border-style"></div>
    <div class="border border-style1"></div>
    <div class="border-style2">
      <b-img src="@/assets/goldSeller/clip.png" class="w-100 h-100" />
    </div>
    <!-- <div class="border border-style"></div>
    <div class="border border-style1"></div> -->
    <!-- <div class="border-style2">
      <b-img src="@/assets/goldSeller/clip.png" class="w-100" />
    </div> -->
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.movie-border {
  position: relative;
  /* width: 100%; */
  height: 50vh;
}
.border-style {
  position: absolute;
  height: 40vh;
  width: 100%;
  border-radius: 2rem;
}

.border-style1 {
  position: absolute;
  height: 40vh;
  width: 95%;
  border-radius: 2rem;
  margin-right: -30px;
  margin-top: 8px;
}

.border-style2 {
  position: absolute;
  height: 38vh;
  width: 90%;
  border-radius: 5rem;
  margin-left: 35px;
  margin-top: 6px;
}
.border {
  border: 2px solid #a87c4f !important;
}

@media (min-width: 1440px) {
  .border-style {
    position: absolute;
    height: 65vh;
    width: 100%;
    border-radius: 5rem;
  }

  .border-style1 {
    position: absolute;
    height: 65vh;
    width: 95%;
    border-radius: 5rem;
    margin-right: -70px;
    margin-top: 8px;
  }

  .border-style2 {
    position: absolute;
    height: 65vh;
    width: 90%;
    border-radius: 5rem;
    margin-left: 86px;
    margin-top: -8px;
  }
}
</style>
