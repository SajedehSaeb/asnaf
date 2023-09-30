
<template>
  <div class="news pb-2 pt-4 px-3">
    <b-row>
      <b-col cols="12" class="d-flex justify-content-center align-item-center">
        <h4>اخبار ویژه بازار</h4>
      </b-col>
      <b-col cols="12" class="price m-3 px-5">
        <p>قیمت طلا</p>
        <p>قیمت سکه</p>
        <p>قیمت نقره</p>
      </b-col>
      <b-col cols="12" class="date p-0">
        <div class="line"></div>
        <p class="pt-3">سه شنبه 14 شهریور 1402</p>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.news {
  background: linear-gradient(rgb(247, 222, 124, 50%), rgb(178, 127, 43, 50%));
  height: 45vh;
  width: 100%;
  border-radius: 10px;
  display: flex;
  justify-content: space-between;
}

@media (min-width: 1440px) {
  .news {
    height: 65vh;
  }
}

.price {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: end;
}
h4,
p {
  font-family: 'Traffic';
  color: #3c2415;
}

.date {
  display: flex;
  flex-direction: column;
  justify-content: end;
  align-items: center;
}

.line {
  border-top: 2px solid #603913;
  /* border-image: linear-gradient(#c9903f, #493e00 , #c9903f); */
  width: 100%;
  margin-top: 13px;
}
</style>
