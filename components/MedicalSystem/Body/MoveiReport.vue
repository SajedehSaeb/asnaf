
<template>
  <div class="pt-5 pb-5 position-relative">
    <div class="bg-movie-img d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 25.png" />
    </div>
    <div class="d-flex justify-content-center align-item-center">
      <b-button class="movie-btn px-5 py-2">فیلم و صوت</b-button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.movie-btn{
  border-radius: 12px;
  background-color: #9E1F63;
  border: 1px solid #9E1F63;
  font-family: 'b nazanin';
  font-size: 20px;
}

.bg-movie-img{
  position: absolute;
  top: -5%;
  left: 21%;
}
</style>
