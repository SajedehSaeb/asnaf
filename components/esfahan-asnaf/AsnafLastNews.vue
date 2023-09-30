<template>
  <div class="last-total-wrap">
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/union-back.png')"
      class="back1"
    />
    <div class="total-wrap">
      <div class="wrap">
        <div class="caption w-100 my-5">
          <div class="wrap-line">
            <img
              :src="
                require('@/assets/images/asnaf/esfahan-asnaf/line-magenta.png')
              "
            />
            <span class="wrap-line-title text-center">آخرین مطالب</span>
          </div>
        </div>

        <div class="content d-flex flex-wrap">
          <div class="last-news">
            <h6 class="date">23 مرداد 1402</h6>
            <div class="mt-3">
              <h4 class="text-center">
                به منظور امنیت شبکه پروژه آمارگیری از مشاغل کشور برگزار <br />شد
                ; رایزنی موسسه بانک اطلاعات مرجع ایران با کارشناسان <br />
                پلیس فتا
              </h4>
            </div>
            <div class="description d-flex flex-wrap">
              <img
                :src="require('@/assets/images/asnaf/news/fata.png')"
                alt="news"
                class="fata-logo"
              />
              <div class="wrap-article1">
                <p class="mb-0 text-justify article-1">
                  لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان
                  و سه درصد گذشته، حال و آینده شناخت فراوان جامعه و متخصصان را
                  می لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و
                  سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد کتابهای
                  زیادی در شصت و سه درصد گذشته، حال و آینده شناخت فراوان جامعه و
                  متخصصان را می طلبد تا با نرم افزارها شناخت بیشتری را برای
                  طراحان رایانه ای علی الخصوص طراحان خلاقی و فرهنگ پیشرو در زبان
                  فارسی ایجاد کرد.
                </p>
              </div>
            </div>
            <p class="mb-0 text-justify article-2">
              لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با
              استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله
              در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد
              نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد.
              طراحان رایانه ای علی الخصوص طراحان خلاقی و فرهنگ پیشرو در زبان
              فارسی ایجاد کرد.
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
                <div class="single-content mt-1">
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
  </div>
</template>

<script>
export default {
  name: 'AsnafLastNews',
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
.last-total-wrap {
  position: relative;
  .back1 {
    position: absolute;
    right: 0;
    top: 3%;
    @media screen and (max-width: 578px) {
      display: none;
    }
  }
  .total-wrap {
    width: 60%;
    margin: 0 auto;
    .wrap {
      .caption {
        .wrap-line {
          position: relative;
          display: flex;
          justify-content: center;
          &-title {
            background-image: linear-gradient(
              270deg,
              hsl(182deg 97% 15%) 0%,
              hsl(182deg 96% 18%) 11%,
              hsl(182deg 95% 20%) 22%,
              hsl(182deg 94% 23%) 33%,
              hsl(182deg 93% 25%) 44%,
              hsl(182deg 91% 28%) 56%,
              hsl(182deg 90% 31%) 67%,
              hsl(182deg 89% 34%) 78%,
              hsl(182deg 87% 36%) 89%,
              hsl(182deg 86% 39%) 100%
            );
            color: white;
            font-size: 25px;
            position: absolute;
            top: 55%;
            border-radius: 0 0 30px 30px;
            padding: 13px 40px;
            -webkit-box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
            -moz-box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
            box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
            font-family: 'B nazanin';
          }

          img {
            width: 100%;
          }
        }
      }
      .content {
        margin-top: 80px;
        .article-1,
        .article-2 {
          color: rgb(160, 159, 159);
          font-size: 15px;
        }
        &-content {
          width: 50%;
        }
        .last-news {
          width: 60%;
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
            .wrap-article1 {
              width: 40%;
              @media screen and (max-width: 768px) {
                width: 100%;
              }
              .article-1 {
                width: 100%;
              }
            }
            .fata-logo {
              width: 60%;
              height: 300px;
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
          width: 35%;
          @media screen and (max-width: 992px) {
            width: 100%;
          }
          .wrap-news {
            .single {
              border-bottom: 1px solid rgba(179, 178, 178, 0.226);
              &-content {
                width: 50%;
                @media screen and (max-width: 768px) {
                  width: 100%;
                }
              }
              .image {
                width: 50%;
                @media screen and (max-width: 768px) {
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
}
</style>
