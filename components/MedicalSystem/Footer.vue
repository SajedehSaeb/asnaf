<template>
  <div>
    <MedicalSystemTopFooter />
    <div class="footer d-flex justify-content-center align-item-center py-5">
      <div class="footer-item">
        <b-row>
          <b-col class="display" cols="12" sm="6" md="4" lg="2">
            <b-row>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center text-center"
              >
                <b-img src="@/assets/medical/Asset 6.png" />
              </b-col>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center text-center"
              >
                <p>پست الکترونیک</p>
              </b-col>
            </b-row>
          </b-col>
          <b-col class="display" cols="12" sm="6" md="4" lg="2">
            <b-row>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center"
              >
                <b-img src="@/assets/medical/Asset 5.png" />
              </b-col>
              <b-col cols="12" class="text-center">
                <p>سامانه صدور و تمدید پروانه مطب</p>
              </b-col>
            </b-row>
          </b-col>
          <b-col class="display" cols="12" sm="6" md="4" lg="2">
            <b-row>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center"
              >
                <b-img src="@/assets/medical/Asset 4.png" />
              </b-col>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center text-center"
              >
                <p>بیمه تامین اجتماعی</p>
              </b-col>
            </b-row>
          </b-col>
          <b-col class="display" cols="12" sm="6" md="4" lg="2">
            <b-row>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center"
              >
                <b-img src="@/assets/medical/Asset 3.png" />
              </b-col>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center text-center"
              >
                <p>درخواست امضای الکترونیک</p>
              </b-col>
            </b-row>
          </b-col>
          <b-col class="display" cols="12" sm="6" md="4" lg="2">
            <b-row>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center"
              >
                <b-img src="@/assets/medical/Asset 2.png" />
              </b-col>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center text-center"
              >
                <p>سامانه مکاتبات اداری</p>
              </b-col>
            </b-row>
          </b-col>
          <b-col class="display" cols="12" sm="6" md="4" lg="2">
            <b-row>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center"
              >
                <b-img src="@/assets/medical/Asset 1.png" />
              </b-col>
              <b-col
                cols="12"
                class="d-flex justify-content-center align-items-center text-center"
              >
                <p>سامانه درخواست پیام کوتاه</p>
              </b-col>
            </b-row>
          </b-col>
        </b-row>
        <!-- <b-row class="mt-2">
          <b-col class="display">
            <p>سامانه درخواست پیام کوتاه</p>
          </b-col>
          <b-col class="display">
            <p>سامانه مکاتبات اداری</p>
          </b-col>
          <b-col class="display">
            <p>درخواست امضای الکترونیک</p>
          </b-col>
          <b-col class="display">
            <p>بیمه تامین اجتماعی</p>
          </b-col>
          <b-col class="text-center">
            <p>سامانه صدور و تمدید پروانه مطب</p>
          </b-col>
          <b-col class="display">
            <p>پست الکترونیک</p>
          </b-col>
        </b-row> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.footer {
  background-color: #2e3743;
}
.footer-item {
  width: 65%;
}

.display {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

P {
  color: white;
  font-family: 'Traffic';
  font-size: 12px;
}
</style>
