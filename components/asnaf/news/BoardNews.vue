<template>
  <div class="total-wrap">
    <img :src="require('@/assets/images/asnaf/news/back.png')" class="back1" />
    <img :src="require('@/assets/images/asnaf/news/back2.png')" class="back2" />
    <img :src="require('@/assets/images/asnaf/news/back3.png')" class="back3" />
    <div class="wrap">
      <div class="caption w-100 my-5">
        <div class="wrap-line">
          <HeaderCaption title="اخبار هیئت رئیسه اتاق اصناف ایران" />

          <div class="head">
            <div
              class="head-content d-flex flex-wrap justify-content-between"
            >
              <h2 class="title-news">آخرین اخبار</h2>
              <b-button class="see-btn"> مشاهده همه </b-button>
            </div>
          </div>
        </div>
      </div>

      <div class="content d-flex flex-wrap">
        <div class="last-news">
          <h6 class="date">23 مرداد 1402</h6>
          <div class="mt-3">
            <h4 class="text-center">
              به منظور امنیت شبکه پروژه آمارگیری از مشاغل کشور برگزار <br />شد ;
              رایزنی موسسه بانک اطلاعات مرجع ایران با کارشناسان <br />
              پلیس فتا
            </h4>
          </div>
          <div class="description d-flex flex-wrap">
            <img
              :src="require('@/assets/images/asnaf/news/fata.png')"
              alt="news"
              class="fata-logo"
            />
            <p class="mb-0 text-justify article-1">
              لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان که
              لازم است و برای شرایط فعلی تکنولوژی مورد کتابهای زیادی در شصت لورم
              ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان که لازم
              است و برای شرایط فعلی تکنولوژی مورد کتابهای زیادی در شصت و سه درصد
              گذشته، حال و آینده شناخت فراوان جامعه و متخصصان را می طلبد تا با
              نرم افزارها شناخت بیشتری را برای طراحان رایانه ای علی الخصوص
              طراحان خلاقی و فرهنگ پیشرو در زبان فارسی ایجاد کرد.
            </p>
          </div>
          <p class="mb-0 text-justify article-2">
            لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
            استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در
            ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و
            کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد. طراحان رایانه
            ای علی الخصوص طراحان خلاقی و فرهنگ پیشرو در زبان فارسی ایجاد کرد.
          </p>
        </div>
        <div class="vertical-line">
          <div class="line"></div>
        </div>
        <div class="observe-all">
          <div class="wrap-news">
            <div
              v-for="(item, index) in items"
              :key="index"
              class="single d-flex flex-wrap justify-content-between py-3"
            >
              <div class="mt-1 desc">
                <p class="caption text-justify mb-0">{{ item.title }}</p>
                <p class="date mt-2 mb-0">{{ item.date }}</p>
              </div>
              <div class="image d-flex justify-content-center">
                <div class="wrap-img">
                  <img
                    :src="require(`@/assets/images/asnaf/news/${item.image}`)"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderCaption from '~/components/asnaf/common/HeaderCaption.vue'
export default {
  name: 'BoardNews',
  components: { HeaderCaption },
  data() {
    return {
      items: [
        {
          title: 'روز پزشک گرامی باد',
          image: 'doctor.jpg',
          date: '23 مرداد 1402',
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است',
          image: 'amar.png',
          date: '23 مرداد 1402',
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است',
          image: 'fata.png',
          date: '23 مرداد 1402',
        },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.total-wrap {
  position: relative;
  .back1 {
    position: absolute;
    left: 0;
    bottom: -18%;
    z-index: -1;
    @media screen and (max-width: 768px) {
      display: none;
    }
  }
  .back2 {
    position: absolute;
    top: 0;
    left: 10%;
    @media screen and (max-width: 768px) {
      display: none;
    }
  }
  .back3 {
    position: absolute;
    right: 3%;
    top: 33%;
    @media screen and (max-width: 768px) {
      display: none;
    }
  }
  .wrap {
    width: 70%;
    margin: 0 auto;
    .caption {
      .wrap-line {
        position: relative;
        font-family: 'B nazanin';
        .head {
          position: absolute;
          top: 100%;
          width: 100%;
          height: 100%;
          padding: 0 60px;
          &-content {
            margin-top: 1rem;
            @media screen and (max-width: 1200px) {
              margin-top: 90px;
            }
          }

          .see-btn {
            background-color: #f04d3b;
            border: none;
            border-radius: 0px;
            padding: 0 30px;
            height: 55px;
            font-weight: bold;
            @media screen and (max-width: 992px) {
              font-size: 12px !important;
              padding: 0 15px;
              height: 40px;
            }
          }
          .title-news {
            font-size: 35px;
            font-weight: bold;
            position: relative;
            font-family: 'B nazanin';
            @media screen and (max-width: 992px) {
              font-size: 20px;
            }
            &::before {
              position: absolute;
              content: '';
              right: 0;
              width: 10%;
              bottom: 0;
              height: 3px;
              background-color: #f04d3b;
              border-radius: 5px;
              @media screen and (max-width: 1100px) {
                bottom: -10px;
              }
              @media screen and (max-width: 992px) {
                bottom: -18px;
              }
            }
            &::after {
              position: absolute;
              content: '';
              right: 20%;
              width: 35%;
              bottom: 0;
              height: 3px;
              background-color: #f04d3b;
              border-radius: 5px;
              @media screen and (max-width: 1100px) {
                bottom: -10px;
              }
              @media screen and (max-width: 992px) {
                bottom: -18px;
              }
            }
          }
        }
      }
    }
    .content {
      margin-top: 130px;
      @media screen and (max-width:992px) {
        margin-top: 180px;
      }
      .article-1,
      .article-2 {
        color: rgb(160, 159, 159);
        font-size: 15px;
      }
      .last-news {
        width: 57%;
        @media screen and (max-width: 992px) {
          width: 100%;
        }
        h4 {
          line-height: 1.5;
        }
        .date {
          color: #f04d3b;
          text-align: center;
          font-size: 13px;
        }
        .description {
          .fata-logo {
            width: 60%;
            height: 300px;
            @media screen and (max-width: 768px) {
              width: 100%;
            }
          }
          .article-1 {
            width: 40%;
            @media screen and (max-width: 768px) {
              width: 100%;
            }
          }
        }
      }
      .vertical-line {
        width: 5%;
        display: flex;
        justify-content: center;
        .line {
          width: 1px;
          height: 100%;
          background-color: #f04d3b;
        }
      }
      .observe-all {
        width: 38%;
        @media screen and (max-width: 992px) {
          width: 100%;
        }
        .wrap-news {
          .single {
            border-bottom: 1px solid rgba(179, 178, 178, 0.226);
            .desc {
              width: 50%;
              @media screen and (max-width: 578px) {
                width: 100%;
              }
            }
            .image {
              width: 50%;
              @media screen and (max-width: 578px) {
                width: 100%;
              }
            }
            .caption {
              font-size: 15px;
              font-weight: bold;
            }
            .date {
              font-size: 12px;
              color: #f04d3b;
              text-align: right;
            }
            .wrap-img {
              width: 185px;
              height: auto;
              img {
                width: 100%;
                height: 100%;
              }
            }
          }
        }
      }
    }
  }
}
</style>
