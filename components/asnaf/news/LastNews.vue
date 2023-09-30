<template>
  <div class="last-news">
    <img :src="require('@/assets/images/asnaf/news/tools.png')" class="back1" />
    <img :src="require('@/assets/images/asnaf/gear.png')" class="back2" />
    <img
      :src="require('@/assets/images/asnaf/news/long-gear.png')"
      class="back3"
    />
    <div class="wrap">
      <HeaderCaption title="آخرین اخبار"/>
      <b-row class="wrap-news">
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
              <span class="caption">{{ item.caption }}</span>
              <p class="content">{{ item.content }}</p>
              <p class="date mb-0">{{ item.date }}</p>
            </div>
          </div>
        </b-col>
      </b-row>
      <div class="d-flex justify-content-center align-items-center mt-5 mb-4">
        <b-button
          class="arshive px-3 py-2 d-flex justify-content-center align-items-center"
        >
          <span>آرشیو</span>
          <div class="wrap-arrow mt-1">
            <i class="icon-keyboard_arrow_left"></i
            ><i class="icon-keyboard_arrow_left second"></i></div
        ></b-button>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderCaption from '~/components/asnaf/common/HeaderCaption.vue'
export default {
  name: 'LastNews',
  components: { HeaderCaption },
  data() {
    return {
      category: [
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',

          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',

          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
        {
          caption: 'عنوان خبر',
          date: '27شهریور1402',
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله ',
        },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.last-news {
  position: relative;
  .back1 {
    position: absolute;
    left: 3%;
    top: 20%;
  }
  .back2 {
    position: absolute;
    left: 5%;
    bottom: 7%;
  }
  .back3 {
    position: absolute;
    right: 7%;
    top: 0;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
  .wrap {
    width: 70%;
    margin: 0 auto;
    font-family: 'B nazanin';
    .wrap-news{
      margin-top: 100px;
    }
    .arshive {
      background-color: #9e1f63;
      border: none;
      border-radius: 8px;
      font-size: 12px;
      .wrap-arrow {
        position: relative;
        .second {
          position: absolute;
          left: -50%;
          top: 20%;
        }
      }
    }
    .single {
      -webkit-box-shadow: -1px 0px 7px 3px rgba(173, 171, 173, 1);
      -moz-box-shadow: -1px 0px 7px 3px rgba(173, 171, 173, 1);
      box-shadow: -1px 0px 7px 3px rgba(173, 171, 173, 1);
      text-align: right;
      .wrap-img {
       width: 30%;
       @media screen and (max-width:768px) {
        width: 100%;
       }
        img {
          width: 100%;
          height: 100%;
        }
      }
      .wrap-content{
        width: 70%;
        @media screen and (max-width:768px) {
        width: 100%;
       }
      }
      .caption {
        font-size: 14px;
      }
      .content {
        font-size: 14px;
      }
      .date {
        font-size: 11px;
        text-align: left;
        color: rgb(165, 165, 165);
      }
    }
  }
}
</style>
