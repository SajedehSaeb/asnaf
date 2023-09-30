<template>
  <div class="total-wrap">
    <div class="wrap mt-5">
      <img
        :src="require('@/assets/images/asnaf/tehran-asnaf/line-magenta.png')"
        class="w-100"
      />
      <img
        :src="require('@/assets/images/asnaf/tehran-asnaf/government-back.png')"
        class="back1"
      />
      <div class="wrap-content d-flex flex-wrap mt-2">
        <div class="government">
          <button class="title-btn">دولت و مجلس</button>
          <div class="options mt-4">
            <div
              v-for="(item, index) in government"
              :key="index"
              class="single d-flex"
            >
              <img :src="require('@/assets/images/asnaf/news/1.jpg')" />
              <div class="pr-2">
                <p class="description mb-0">{{ item.title }}</p>
                <p class="date mb-0">{{ item.date }} - {{ item.time }}</p>
              </div>
            </div>
          </div>
        </div>
        <div class="asnaf">
          <button class="title-btn">اصناف در آینه رسانه</button>
          <div class="options mt-4">
            <div
              v-for="(item, index) in government"
              :key="index"
              class="single d-flex"
            >
              <img :src="require('@/assets/images/asnaf/news/1.jpg')" />
              <div class="pr-2">
                <p class="description mb-0">{{ item.title }}</p>
                <p class="date mb-0">{{ item.date }} - {{ item.time }}</p>
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
  name: 'AsnafGovernment',
  data() {
    return {
      government: [
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت',
          date: '23 مرداد 1402',
          time: '6:25',
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت',
          date: '23 مرداد 1402',
          time: '6:25',
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت',
          date: '23 مرداد 1402',
          time: '6:25',
        },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.total-wrap {
  position: relative;
  .wrap {
    width: 60%;
    margin: 0 auto;
    .back1 {
      position: absolute;
      left: 2%;
      bottom: 0;
    }
    .title-btn {
      margin-right: 50px;
      @media screen and (max-width: 992px) {
        margin-right: 0;
      }
      background-image: linear-gradient(
        90deg,
        hsl(285deg 18% 43%) 0%,
        hsl(285deg 19% 41%) 11%,
        hsl(285deg 20% 39%) 22%,
        hsl(285deg 22% 37%) 33%,
        hsl(285deg 23% 35%) 44%,
        hsl(285deg 24% 33%) 56%,
        hsl(285deg 26% 31%) 67%,
        hsl(285deg 28% 29%) 78%,
        hsl(285deg 30% 27%) 89%,
        hsl(285deg 32% 25%) 100%
      );
      border: none;
      color: white;
      font-family: 'B nazanin';
      padding: 20px 30px;
      border-radius: 17px;
      font-weight: bold;
      font-size: 18px;
    }
    &-content {
      text-align: right;
      .options {
        .single {
          line-height: 1.5;
          border-bottom: 1px solid rgba(228, 223, 223, 0.61);
          padding: 8px 0;
          @media screen and (max-width: 578px) {
            flex-direction: column;
            justify-content: center;
            align-items: center;
          }
          &:last-child {
            border-bottom: none;
          }

          &:nth-child(2) {
            .description {
              color: #ffac52;
            }
          }
          img {
            width: 120px;
            height: 70px;
          }
          .date {
            color: rgb(172, 172, 172);
            font-size: 12px;
          }
          .description {
            font-size: 14px;
            font-weight: bold;
          }
        }
      }
      .government,
      .asnaf {
        width: 50%;
        padding: 0 50px;
        @media screen and (max-width: 992px) {
          width: 100%;
          padding: 0;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;
        }
      }
      .government {
        border-left: 2px dashed rgba(218, 216, 216, 0.404);

        @media screen and (max-width: 992px) {
          width: 100%;
          border-left: none;
        }
      }
      // .wrap-line {
      //   width: 10%;
      //   display: flex;
      //   justify-content: center;
      //   align-items: center;
      //   .line {
      //     width: 2px;
      //     border-right: 2px dashed rgba(218, 216, 216, 0.404);
      //     height: 100%;
      //   }
      // }
    }
  }
}
</style>
