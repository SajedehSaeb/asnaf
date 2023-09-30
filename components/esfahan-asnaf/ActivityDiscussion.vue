<template>
  <div class="total-wrap-activity">
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/discussion-back.png')"
      class="back1"
    />
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/activity-back.png')"
      class="back2"
    />
    <div class="wrap">
      <div>
        <img
          :src="require('@/assets/images/asnaf/esfahan-asnaf/line-magenta.png')"
          alt="news"
          class="w-100"
        />
      </div>
      <div class="wrap-content d-flex flex-wrap justify-content-between">
        <div class="activity-wrap">
          <div class="d-flex justify-content-center">
            <b-button class="title-btn">فعالیت کاربردی</b-button>
          </div>
          <div class="mt-3">
            <b-row v-for="(item, index) in activity" :key="index">
              <div class="single d-flex">
                <div class="px-1 py-1">
                  <p class="content mb-0">{{ item.content }}</p>
                  <p class="day mb-0">{{ item.day }}</p>
                </div>
              </div>
            </b-row>
          </div>
        </div>
        <div class="discussion-wrap">
          <div class="d-flex justify-content-center">
            <b-button class="title-btn">گفتگو</b-button>
          </div>
          <div class="mt-3">
            <b-row
              v-for="(item, index) in mostVisited"
              :key="index"
              class="single mt-2"
            >
              <div class="single-content d-flex pb-2">
                <div class="wrap-img">
                  <img
                    :src="require('@/assets/images/asnaf/news/1.jpg')"
                    alt="news"
                  />
                </div>
                <div class="pr-2">
                  <p class="content">{{ item.content }}</p>
                  <p class="family mb-0">{{ item.family }}</p>
                </div>
              </div>
            </b-row>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

    <script>
export default {
  name: 'ActivityDiscussion',
  data() {
    return {
      activity: [
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم .',
          day: '6 روز قبل',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است.',
          day: '6 روز قبل',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است.',
          day: '6 روز قبل',
        },
        {
          content: 'لورم ایپسوم متن ساختگی با تولید سادگی .',
          day: '6 روز قبل',
        },
        {
          content: 'لورم ایپسوم متن ساختگی با تولید .',
          day: '6 روز قبل',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با .',
          day: '6 روز قبل',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است.',
        },
      ],
      mostVisited: [
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و  ',
          family: 'مولایی',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و  ',

          family: 'مولایی',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و  ',

          family: 'مولایی',
        },
        {
          content:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ و با استفاده از طراحان گرافیک است. چاپگرها و  ',

          family: 'مولایی',
        },
      ],
    }
  },
}
</script>
<style scoped lang="scss">
.total-wrap-activity {
  position: relative;
  .back1 {
    position: absolute;
    left: 5%;
    @media screen and (max-width: 578px) {
      display: none;
    }
  }
  .back2 {
    position: absolute;
    right: 5%;
    top: 4%;
    @media screen and (max-width: 578px) {
      display: none;
    }
  }
  .wrap {
    width: 60%;
    margin: 0 auto;
    &-content {
      .activity-wrap {
        width: 50%;
        padding: 0 50px;
        border-left: 2px dashed rgba(218, 216, 216, 0.404);
        @media screen and (max-width: 992px) {
          width: 100%;
          border-left: none;
          padding: 0;
        }
        .single {
          line-height: 1.75;
        }
      }
      .discussion-wrap {
        width: 50%;
        padding: 0 50px;
        @media screen and (max-width: 992px) {
          width: 100%;
          padding: 0;
        }
        .single {
          &:nth-child(1) {
            border-bottom: 1px solid rgba(219, 219, 219, 0.705);
          }
          &:nth-child(3) {
            border-bottom: 1px solid rgba(219, 219, 219, 0.705);
            margin-top: 50px !important;
          }
          &-content {
            @media screen and (max-width: 578px) {
              flex-direction: column;
              justify-content: center;
              align-items: center;
            }
          }
        }
      }
      .title-btn {
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
        border: none;
        color: white;
        font-family: 'B nazanin';
        padding: 20px 30px;
        border-radius: 17px;
        font-weight: bold;
        font-size: 20px;
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
        text-align: right;
        border-radius: 3px;
        .day {
          font-size: 13px;
          color: rgb(155, 154, 154);
          font-family: 'Traffic';
        }
        .wrap-img {
          width: 150px;
          height: 90px;
          border-radius: 50%;
          border: 6px solid #dadada;
          @media screen and (max-width: 578px) {
            width: 100px;
            height: 100px;
          }
          img {
            width: 100%;
            height: 100%;
            border-radius: 50%;
          }
        }
        .content {
          font-size: 14px;
          font-weight: 400;
          font-family: 'Traffic';
        }
        .family {
          font-size: 12px;
          color: rgba(155, 152, 152, 0.795);
        }
      }
    }
  }
}
</style>
