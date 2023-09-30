<template>
  <div class="news-room">
    <img
      :src="require('@/assets/images/asnaf/news/room-back.png')"
      class="back1"
    />
    <div class="wrap">
      <HeaderCaption title="اخبار اتاق اصناف سراسر کشور" />
      <b-row class="news-room-options">
        <b-col
          v-for="(item, index) in category"
          :key="index"
          cols="12"
          lg="6"
          md="12"
          class="mt-2"
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
        </b-col>
      </b-row>
    </div>
  </div>
</template>

  <script>
import HeaderCaption from '~/components/asnaf/common/HeaderCaption.vue'
export default {
  name: 'AsnafNews',
  components: { HeaderCaption },
  data() {
    return {
      category: [
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
.news-room {
  position: relative;
  &-options{
    margin-top: 100px;
  }
  .back1 {
    position: absolute;
    left: 0;
    top: -23%;
    @media screen and (max-width: 768px) {
      display: none;
    }
  }
  .wrap {
    width: 70%;
    margin: 0 auto;
    font-family: 'B nazanin';
    .single {
      background-color: #f2f2f2;
      text-align: right;
      border-radius: 3px;
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
      .wrap-content{
        width: 70%;
        @media screen and (max-width: 768px) {
          width: 100%;
        }
      }
      .content {
        font-size: 14px;
        font-weight: 400;
        font-family: 'B nazanin';
      }
    }
  }
}
</style>
