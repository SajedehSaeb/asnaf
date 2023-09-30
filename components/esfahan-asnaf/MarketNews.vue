<template>
  <div class="market-total-wrap">
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/activity-back.png')"
      class="back1"
    />
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/activity-back.png')"
      class="back2"
    />
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/discussion-back.png')"
      class="back3"
    />
    <div class="wrap mt-4">
      <div class="caption">
        <img
          :src="require('@/assets/images/asnaf/esfahan-asnaf/line-magenta.png')"
          class="w-100"
        />
        <span class="title d-flex justify-content-center align-items-center">
          بازار در اخبار
        </span>
      </div>
      <div class="wrap-options">
        <div class="wrap-options-content">
          <b-row>
            <b-col
              v-for="(item, index) in items"
              :key="index"
              cols="12"
              class="single mt-3 px-0"
            >
              <div class="wrap-content d-flex">
                <div class="wrap-img">
                  <img :src="require('@/assets/images/asnaf/room.jpg')" />
                  <div class="date">
                    <p class="mb-0 font-weight-bold">13</p>
                    <p class="mb-0 day">شهریور</p>
                  </div>
                </div>
                <div class="content p-2">
                  <p class="title-content">{{ item.title }}</p>
                  <h5>{{ item.caption }}</h5>
                  <p class="text-justify title-content">{{ item.description }}</p>
                </div>
              </div>
            </b-col>
          </b-row>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MarketNews',
  data() {
    return {
      items: [
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان و سه درصد گذشته',
          caption: 'لورم ایپسوم متن ساختگی با تولید',
          description:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد.',
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان و سه درصد گذشته',
          caption: 'لورم ایپسوم متن ساختگی با تولید',
          description:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد.',
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان و سه درصد گذشته',
          caption: 'لورم ایپسوم متن ساختگی با تولید',
          description:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد.',
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی و با در ستون و سطرآنچنان و سه درصد گذشته',
          caption: 'لورم ایپسوم متن ساختگی با تولید',
          description:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که لازم است و برای شرایط فعلی تکنولوژی مورد نیاز و کاربردهای متنوع با هدف بهبود ابزارهای کاربردی می باشد.',
        },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.market-total-wrap {
  position: relative;
  .back1 {
    position: absolute;
    top: 0;
    left: 16%;
    opacity: 0.5;
  }
  .back2 {
    position: absolute;
    left: 3%;
    bottom: 0;
  }
  .back3 {
    position: absolute;
    right: 1%;
    bottom: 0;
  }
  .wrap {
    width: 60%;
    margin: 0 auto;
    .caption {
      margin: 0 auto;
      position: relative;
      display: flex;
      justify-content: center;
      .title {
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
        font-family: 'B nazanin';
        position: absolute;
        top: 55%;
        border-radius: 0 0 30px 30px;
        padding: 13px 40px;
        -webkit-box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
        -moz-box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
        box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
      }
    }
    &-options {
      margin-top: 100px;
      &-content {
        width: 80%;
        margin: 0 auto;
        background-color: #f2f2f2;
        padding-bottom: 10px;
        @media screen and (max-width: 1200px) {
          width: 100%;
        }
        @media screen and (max-width: 768px) {
          width: 100%;
        }
        .row {
          width: 95%;
          margin: 0 auto;
          .single {
            text-align: right;
            -webkit-box-shadow: 4px 4px 7px 0px rgba(179, 170, 179, 1);
            -moz-box-shadow: 4px 4px 7px 0px rgba(179, 170, 179, 1);
            box-shadow: 4px 4px 7px 0px rgba(179, 170, 179, 1);
            background-color: #ffffff;
            .wrap-content {
              @media screen and (max-width: 768px) {
                flex-direction: column;
              }
            }
            .wrap-img {
              position: relative;
              width: 30%;
              @media screen and (max-width: 768px) {
                width: 100%;
              }
              img {
                width: 100%;
                height: 100%;
                border: 5px solid #362365;
              }
              .date {
                position: absolute;
                top: 5%;
                right: -5%;
                background-color: #ffffff;
                border: 3px solid #1c39bb;
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                padding: 3px;
                .day {
                  color: grey;
                }
              }
            }
            .content {
              width: 70%;
              font-size: 15px;
              font-family: 'IRANSans';
              @media screen and (max-width: 768px) {
                width: 100%;
              }
            }
          }
        }
      }
    }
  }


  .title-content{
    color: gray;
    font-family: 'IRANSans';
  }
}
</style>
