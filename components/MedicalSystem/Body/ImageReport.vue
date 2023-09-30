
<template>
  <div class="mb-5 position-relative">
    <div class="bg-report-img">
      <b-img src="@/assets/medical/Asset 22.png" />
    </div>
    <div class="bg-report-img1">
      <b-img src="@/assets/medical/Asset 24.png" />
    </div>
    <div class="bg-report-img2">
      <b-img src="@/assets/medical/Asset 22.png" />
    </div>
    <div class="d-flex justify-content-center align-item-center">
      <div class="image-reports py-2">
        <p>گزارش تصویری</p>
      </div>
    </div>
    <div class="d-flex justify-content-center align-item-center mt-4">
      <b-row class="w-70">
        <b-col
          cols="12"
          lg="4"
          class="d-flex justify-content-center align-item-center my-3"
        >
          <div class="image-border"></div>
          <div class="image-frame">
            <div
              class="h-100 w-100 d-flex justify-content-center align-item-center p-3"
            >
              <b-img src="@/assets/medical/55.jpg" class="image-frame1" />
            </div>
          </div>
        </b-col>
        <b-col
          cols="12"
          lg="4"
          class="d-flex justify-content-center align-item-center my-3"
        >
          <div class="image-border"></div>
          <div class="image-frame">
            <div
              class="h-100 w-100 d-flex justify-content-center align-item-center p-3"
            >
              <b-img src="@/assets/medical/44.jpg" class="image-frame1" />
            </div>
          </div>
        </b-col>
        <b-col
          cols="12"
          lg="4"
          class="d-flex justify-content-center align-item-center my-3"
        >
          <div class="image-border"></div>
          <div class="image-frame">
            <div
              class="h-100 w-100 d-flex justify-content-center align-item-center p-3"
            >
              <b-img src="@/assets/medical/66.jpg" class="image-frame1" />
            </div>
          </div>
        </b-col>
      </b-row>
    </div>
    <div class="mt-3">
      <b-row class="d-flex justify-content-center align-item-center w-100">
        <b-button class="btn-style px-3">
          <b-img src="@/assets/medical/Asset 33.png" />
          آرشیو
        </b-button>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>

.w-70{
  width: 65%;
}
.image-reports {
  background-color: #662d91;
  width: 50%;
  color: white;
  text-align: center;
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  box-shadow: 4px 5px 8px rgb(79, 79, 79);
  z-index: 1;
}

@media (min-width: 768px) {
  .image-reports {
    width: 20%;
  }
}

.image-border {
  position: relative;
  border: 1px solid #662d91;
  border-radius: 30px;
  height: 27vh;
  width: 17vw;
}

.image-frame {
  position: absolute;
  top: -8%;
  left: 14%;
  background-color: #662d91;
  border-radius: 30px;
  height: 27vh;
  width: 17vw;
}

.image-frame1 {
  border: 1px solid white;
  border-radius: 20px;
  height: 100%;
  width: 95%;
}

@media (max-width: 768px) {
  .image-border {
    border-radius: 30px;
    height: 27vh;
    width: 60vw;
  }

  .image-frame {
    height: 27vh;
    width: 60vw;
  }
}

@media (min-width: 1024px) {
  .image-reports {
    width: 13%;
  }

  .image-frame {
    position: absolute;
    top: -8%;
    left: 20%;
    background-color: #662d91;
    border-radius: 30px;
    height: 27vh;
    width: 17vw;
  }
}

.btn-style {
  background-color: #a01f62;
  border-color: #a01f62;
  border-radius: 10px;
}

.bg-report-img {
  position: absolute;
  bottom: 6%;
  left: 16.5%;
}

.bg-report-img1 {
  position: absolute;
  bottom: -17%;
  right: 0;
}

.bg-report-img2{
  position: absolute;
  top: 3%;
  right: 20%;
}
</style>
