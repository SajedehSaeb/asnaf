<template>
  <div
    dir="rtl"
    class="d-flex justify-content-center align-item-center purple-border"
  >
    <b-row class="w-100">
      <b-col
        cols="12"
        sm="4"
        class="d-flex justify-content-center justify-content-lg-end align-item-center px-5 py-3"
      >
        <p>مکاتبات</p>
      </b-col>
      <b-col
        cols="12"
        sm="4"
        class="d-flex justify-content-center align-item-center border-style py-3"
      >
        <p>پیام های آموزشی</p>
      </b-col>
      <b-col
        cols="12"
        sm="4"
        class="d-flex justify-content-center justify-content-lg-start align-item-center px-5 py-3 text-center"
      >
        <p>قانون پایه های فروشگاهی</p>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.purple-border {
  border-bottom: 10px solid #662d91;
  box-shadow: 0px -8px 16px rgba(128, 128, 128, 0.927);
}

.border-style {
  border-left: 1px dashed #662d91;
  border-right: 1px dashed #662d91;
}

p {
  font-family: 'B nazanin';
  color: #662d91;
  font-size: 25px;
  font-weight: bold;
}

@media (max-width: 425px) {
  .border-style {
    border-left: none;
    border-right: none;
    border-top: 1px dashed #662d91;
    border-bottom: 1px dashed #662d91;
  }
}
</style>
