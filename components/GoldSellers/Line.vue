<template>
  <div class="d-flex justify-content-center align-item-center">
    <div>
      <b-img src="@/assets/goldSeller/circle.png" />
    </div>
    <!-- <div class="circle"></div> -->
    <div class="line"></div>
    <div>
      <b-img src="@/assets/goldSeller/circle.png" />
    </div>

  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.line{
  border-top: 2px solid rgba(247, 222, 124, 0.5);
  /* border-image: linear-gradient(#c9903f, #493e00 , #c9903f); */
  width: 60%;
  margin-top: 13px;
}
.circle{
  height: 15px;
  width: 15px;
  border-radius: 50%;
  background-image: linear-gradient(65deg, #c9903f, #efe295 ,#c9903f);
  border: #c9903f;
  box-shadow: 1px 2px 5px grey;
  /* margin-top: -5px; */
}
</style>
