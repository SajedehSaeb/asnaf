<template>
  <div class="wrap mt-5">
    <div class="wrap-line">
      <img
        :src="require('@/assets/images/asnaf/news/line3.png')"
        alt="news"
        class="line w-100"
      />
    </div>
    <b-row class="options">
      <div class="wrap-category">
        <div class="d-flex justify-content-center">
          <b-button class="title-btn">روابط عمومی های برتر</b-button>
        </div>
        <div class="mt-3">
          <b-row
            v-for="(item, index) in topPublic"
            :key="index"
            class="mt-2 mx-0"
          >
            <div class="single d-flex">
              <div class="wrap-img">
                <img
                  :src="require('@/assets/images/asnaf/news/1.jpg')"
                  alt="news"
                />
              </div>
              <div class="px-2 py-2">
                <p class="content">{{ item.content }}</p>
              </div>
            </div>
          </b-row>
        </div>
      </div>
      <div class="wrap-category">
        <div class="d-flex justify-content-center">
          <b-button class="title-btn">گفتگو</b-button>
        </div>
        <div class="mt-3">
          <b-row
            v-for="(item, index) in discussion"
            :key="index"
            class="mt-2 mx-0"
          >
            <div class="single d-flex">
              <div class="wrap-img">
                <img
                  :src="require('@/assets/images/asnaf/news/1.jpg')"
                  alt="news"
                />
              </div>
              <div class="px-2 py-2">
                <p class="content">{{ item.content }}</p>
              </div>
            </div>
          </b-row>
        </div>
      </div>
      <div class="wrap-category">
        <div class="d-flex justify-content-center">
          <b-button class="title-btn">یادداشت</b-button>
        </div>
        <div class="mt-3">
          <b-row v-for="(item, index) in notes" :key="index" class="mt-2 mx-0">
            <div class="single d-flex">
              <div class="wrap-img">
                <img
                  :src="require('@/assets/images/asnaf/news/1.jpg')"
                  alt="news"
                />
              </div>
              <div class="px-2 py-2">
                <p class="content">{{ item.content }}</p>
              </div>
            </div>
          </b-row>
        </div>
      </div>
    </b-row>
  </div>
</template>

      <script>
export default {
  name: 'TopPublicRelationship',
  data() {
    return {
      topPublic: [
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی  ',
        },
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی  ',
        },
      ],
      discussion: [
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی  ',
        },
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی  ',
        },
      ],
      notes: [
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی  ',
        },
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی  ',
        },
      ],
    }
  },
}
</script>
  <style scoped lang="scss">
.wrap {
  width: 70%;
  margin: 0 auto;
  .options {
    justify-content: space-between;
    @media screen and (max-width: 992px) {
      justify-content: center;
    }
  }
  .wrap-category {
    width: 30%;
    @media screen and (max-width: 992px) {
      width: 100%;
    }
  }
  .title-btn {
    background-color: #2e3192;
    border: none;
    color: white;
    padding: 10px 30px;
    width: 70%;
    border-radius: 17px;
    font-weight: bold;
    margin-top: 15px;
    font-family: 'B nazanin';
    font-size: 20px;
  }

  .single {
    background-color: #f2f2f2;
    text-align: right;
    border-radius: 3px;
    @media screen and (max-width: 992px) {
      width: 100%;
    }
    .wrap-img {
      width: 100px;
      img {
        width: 100%;
        height: 100%;
      }
    }
    .content {
      font-size: 14px;
      font-weight: 400;
      font-weight: bold;
    }
  }
}
</style>
