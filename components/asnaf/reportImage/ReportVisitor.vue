<template>
  <div class="wrap mt-5">
    <div class="wrap-line">
      <img
        :src="require('@/assets/images/asnaf/news/line3.png')"
        alt="news"
        class="line"
      />
    </div>
    <b-row class="justify-content-between mx-0">
      <b-col cols="12" lg="5" class="px-0">
        <div class="d-flex justify-content-center">
          <b-button class="title-btn">گزارش</b-button>
        </div>
        <div class="mt-3">
          <b-row
            v-for="(item, index) in reports"
            :key="index"
            class="mt-2 mx-0"
          >
            <div class="single d-flex flex-wrap">
              <div class="wrap-img">
                <img
                  :src="require('@/assets/images/asnaf/news/1.jpg')"
                  alt="news"
                />
              </div>
              <div class="wrap-content px-2 py-2">
                <p class="content">{{ item.content }}</p>
              </div>
            </div>
          </b-row>
        </div>
      </b-col>
      <b-col cols="12" lg="5" class="px-0">
        <div class="d-flex justify-content-center">
          <b-button class="title-btn">پربازدیدترین ها</b-button>
        </div>
        <div class="mt-3">
          <b-row
            v-for="(item, index) in mostVisited"
            :key="index"
            class="mt-2 mx-0"
          >
            <div class="single d-flex flex-wrap">
              <div class="wrap-img">
                <img
                  :src="require('@/assets/images/asnaf/news/1.jpg')"
                  alt="news"
                />
              </div>
              <div class="wrap-content px-2 py-2">
                <p class="content">{{ item.content }}</p>
              </div>
            </div>
          </b-row>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

    <script>
export default {
  name: 'ReportVisitor',
  data() {
    return {
      reports: [
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
      ],
      mostVisited: [
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
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
  .title-btn {
    background-color: #2e3192;
    border: none;
    color: white;
    padding: 10px 30px;
    border-radius: 17px;
    font-weight: bold;
    font-family: 'B nazanin';
    @media screen and (max-width: 992px) {
      margin-top: 25px;
    }
  }
  &-line {
    @media screen and (max-width: 768px) {
      display: none;
    }
    img {
      width: 100%;
    }
  }
  .single {
    background-color: #f2f2f2;
    text-align: right;
    border-radius: 3px;
    .wrap-content{
      width: 70%;
      @media screen and (max-width: 768px) {
        width: 100%;
      }
    }
    .wrap-img {
      width: 30%;
      @media screen and (max-width: 768px) {
        width: 100%;
      }
      img {
        width: 100%;
        height: 100%;
      }
    }
    .content {
      font-size: 14px;
      font-weight: 400;
    }
  }
}
</style>
