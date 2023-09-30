<template>
  <div class="d-flex justify-content-center align-item-center line-style">
    <div class="circle"></div>
    <div class="line"></div>
    <div class="circle"></div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.line-style{
  margin-bottom: -5px;
}
.line {
  border-top: 1px solid #662d91;
  /* border-image: linear-gradient(#c9903f, #493e00 , #c9903f); */
  width: 75vw;
  margin-top: 13px;
  z-index: 1;
}
.circle {
  height: 8px;
  width: 8px;
  border-radius: 50%;
  background-color: #662d91;
  margin-top: 10px;
  z-index: 1;
}
</style>
