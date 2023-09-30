<template>
  <div dir="rtl">
    <GoldSellersLine />
    <div class="gallery-button ">
      <b-button class="button">گالری فیلم و عکس</b-button>
    </div>

    <div class="mt-3 gallery ">
      <b-row class="w-100">
        <b-col cols="12" xl="6" class="gallery1">
          <b-row class="w-100">
            <b-col
              cols="12"
              class="d-flex justify-content-center align-item-center"
            >
              <b-img src="@/assets/goldSeller/Asset 33.png" class="first-img"/>
            </b-col>
            <b-col cols="12">
              <b-row
                class="d-flex justify-content-center align-item-center"
              >
                <b-img src="@/assets/goldSeller/Asset 38.png" class="m-2"/>
                <b-img src="@/assets/goldSeller/Asset 35.png" class="m-2"/>
                <b-img src="@/assets/goldSeller/Asset 36.png" class="m-2"/>
              </b-row>
            </b-col>
          </b-row>
        </b-col>

        <b-col cols="12" xl="6" class="gallery1">
          <b-row class="w-100">
            <b-col
              cols="12"
              class="d-flex justify-content-center align-item-center"
            >
              <b-img src="@/assets/goldSeller/Asset 33.png" class="first-img"/>
            </b-col>
            <b-col cols="12">
              <b-row
                class="d-flex justify-content-center align-item-center"
              >
                <b-img src="@/assets/goldSeller/Asset 38.png" class="m-2"/>
                <b-img src="@/assets/goldSeller/Asset 35.png" class="m-2"/>
                <b-img src="@/assets/goldSeller/Asset 36.png" class="m-2"/>
              </b-row>
            </b-col>
          </b-row>
        </b-col>

      </b-row>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.gallery-button {
  display: flex;
  justify-content: center;
  align-items: center;
}

.button {
  background-image: linear-gradient(90deg, #c9903f, #efe295);
  border-image: linear-gradient(90deg, #c9903f, #efe295);
  box-shadow: 5px 8px 5px rgba(128, 128, 128, 0.834);
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  width: 65%;
  padding: 10px;
  font-family: 'Traffic';
  font-size: 24px;
  z-index: 1;
}

@media (min-width: 1440px){
  .button{
    width: 16%;
  }
}

@media (max-width: 425px){
  .first-img{
    width: 75vw;
  }
}

.gallery {
  display: flex;
  justify-content: center;
  align-items: center;
}

.gallery1 {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
