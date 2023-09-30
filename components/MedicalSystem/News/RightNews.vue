<template>
  <div class="d-flex justify-content-center align-item-center mt-2">
    <b-row class="d-flex justify-content-center align-item-center w-75">
      <b-col cols="12" md="10" class="div-style">
        <b-row class="note-style"> یادداشت روز </b-row>
      </b-col>
      <b-col
        v-for="(x, i) in items"
        :key="i"
        cols="10"
        md="9"
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
          title: 'اطلاعیه های مهم',
        },
        {
          title: 'آگهی استخدام',
        },
        {
          title: 'اشتراک نشریه سازمان',
        },
        {
          title: 'هشتمین روره انتخابات نظام پزشکی',
        },
        {
          title: 'نسخه الکترونیک',
        },
        {
          title: 'گوداستندینگ',
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
  background-color: #bc8dc0;
  border-radius: 15px;
  font-family: 'b nazanin';
  font-weight: bold;
  font-size: 20px;
  height: 45vh;
}

.note-style {
  background-color: #662d91;
  border-radius: 15px 15px 0 0;
  font-family: 'b nazanin';
  font-weight: 200;
  font-size: 20px;
  height: 5vh;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
}

.div-styles {
  background-color: #9e1f63;
  border-radius: 15px;
  font-family: 'b nazanin';
  font-weight: 200;
  font-size: 15px;
  color: white;
  text-align: center;
}
</style>
