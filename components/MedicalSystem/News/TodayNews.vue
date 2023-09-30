<template>
  <div class="mb-5 position-relative" dir="ltr">
    <div class="bg-news-img d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 26.png" />
    </div>
    <div class="bg-news-img1 d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 29.png" />
    </div>
    <div class="bg-news-img2 d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 27.png" />
    </div>
    <div class="bg-news-img3 d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 30.png" />
    </div>
    <div class="bg-news-img4 d-none d-md-flex">
      <b-img src="@/assets/medical/Asset 31.png" />
    </div>
    <!-- <b-row class="bg-info w-100"> -->
      <b-col cols="12" class="d-flex justify-content-center align-item-center">
        <div class="news py-2">
          <h5>اخبار روز</h5>
        </div>
      </b-col>

      <b-col cols="12" class="mt-5">
        <b-row>
          <b-col
            cols="12"
            lg="3"
          >
            <MedicalSystemNewsLeftNews />
          </b-col>
          <b-col cols="12" lg="6" class="mt-5 mt-lg-0">
            <MedicalSystemNewsLastNews />
          </b-col>
          <b-col cols="12" lg="3">
            <MedicalSystemNewsRightNews />
          </b-col>
        </b-row>
      </b-col>
    <!-- </b-row> -->
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.news {
  background-color: #662d91;
  width: 50%;
  color: white;
  text-align: center;
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  box-shadow: 4px 5px 8px rgb(79, 79, 79);
}

@media (min-width: 768px) {
  .news {
    width: 20%;
  }
}

@media (min-width: 1024px) {
  .news {
    width: 13%;
  }
}

h5 {
  font-family: 'B nazanin';
}

.bg-news-img{
  position: absolute;
  bottom: 5%;
  left: 8%;
}

.bg-news-img1{
  position: absolute;
  bottom: -5%;
  left: 10%;
}

.bg-news-img2{
  position: absolute;
  bottom: 8%;
  left: 23%;
}

.bg-news-img3{
  position: absolute;
  top: -9%;
  right:0;
}

.bg-news-img4{
  position: absolute;
  top: 10.2%;
  left:0;
}
</style>
