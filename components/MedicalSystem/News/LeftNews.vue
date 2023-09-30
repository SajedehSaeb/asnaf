<template>
  <div class="d-flex justify-content-center align-item-center ">
    <b-row class="d-flex justify-content-center align-item-center w-75 ">
      <b-col
        cols="12" md="10"
        class="div-style d-flex justify-content-center align-item-center mb-2 "
      >
        همایش
      </b-col>
      <b-col
        cols="12" md="10"
        class="div-style d-flex justify-content-center align-item-center"
      >
        سمینار
      </b-col>

      <b-col
        v-for="(x, i) in items"
        :key="i"
        cols="10" md="9"
        class="div-styles d-flex justify-content-center align-item-center mt-2 py-2"
      >
        {{ x.title }}
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'انجمن ها',
        },
        {
          title: 'آموزش سلامت همگانی',
        },
        {
          title: 'سامانه آمار',
        },
        {
          title: 'فراخوان-مناقصه-مزایده',
        },
        {
          title: 'همایش ها',
        },
      ],
    }
  },
}
</script>

<style scoped>
.left-news {
  height: 70vh;
}
.div-style {
  background-color: #e2d4b7;
  border-radius: 15px;
  font-family: 'b nazanin';
  font-weight: bold;
  font-size: 20px;
  padding: 35px 15px;
}

.div-styles {
  background-color: #9e1f63;
  border-radius: 15px;
  font-family: 'b nazanin';
  font-weight: 200;
  font-size: 20px;
  color: white;
  text-align: center;
}
</style>
