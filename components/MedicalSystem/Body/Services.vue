<template>
  <div class="service-border">
    <div class="d-flex justify-content-center align-item-center">
      <b-row class="w-100">
        <b-col
          cols="12"
          class="d-flex justify-content-center align-item-center"
        >
          <div class="service py-2">
            <h5>خدمات سازمان</h5>
          </div>
        </b-col>
        <b-col class="d-flex justify-content-center align-item-center mt-5">
          <div class="w-100">
            <b-row>
              <b-col class="display" cols="12" md="3">
                <b-img src="@/assets/medical/Asset 10.png" />
                <p>پرتال فردی پزشک</p>
              </b-col>

              <b-col class="display border-services1" cols="12" md="3">
                <b-img src="@/assets/medical/Asset 9.png" />
                <p>سامانه ثبت نام غیر حضوری</p>
              </b-col>

              <b-col class="display border-services" cols="12" md="3">
                <b-img src="@/assets/medical/Asset 8.png" />
                <p>جستجوی پزشک</p>
              </b-col>

              <b-col class="display" cols="12" md="3">
                <b-img src="@/assets/medical/Asset 7.png" />
                <p>مجوز تبلیغات پزشکی</p>
              </b-col>
            </b-row>
            <!-- <b-row>
              <b-col class="display">
                <p>مجوز تبلیغات پزشکی</p>
              </b-col>
              <b-col class="display border-services">
                <p>جستجوی پزشک</p>
              </b-col>
              <b-col class="display border-services1">
                <p>سامانه ثبت نام غیر حضوری</p>
              </b-col>
              <b-col class="display">
                <p>پرتال فردی پزشک</p>
              </b-col>
            </b-row> -->
          </div>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.service {
  background-color: #662d91;
  width: 13%;
  color: white;
  text-align: center;
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  box-shadow: 4px 5px 8px rgb(79, 79, 79);
}

.service-border {
  border-bottom: 3px solid #662d91;
  border-top: 3px solid #413f99;
  box-shadow: 0px -8px 16px rgba(128, 128, 128, 0.927);
}

.border-services {
  border-right: 1px dashed #7a729b;
  border-left: 1px dashed #7a729b;
}

.border-services1 {
  border-right: 1px dashed #7a729b;
}

@media (max-width: 425px) {
  .service {
    width: 50%;
  }
  .border-services {
    border-right: none;
    border-left: none;
    border-top: 1px dashed #7a729b;
    border-bottom: 1px dashed #7a729b;
  }

  .border-services1 {
    border-right: none;
    border-bottom: 1px dashed #7a729b;
  }
}

.display {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

p {
  font-family: 'B nazanin';
  font-size: 25px;
  font-weight: bold;
  color: #662d91;
}

h5 {
  font-family: 'B nazanin';
}
</style>
