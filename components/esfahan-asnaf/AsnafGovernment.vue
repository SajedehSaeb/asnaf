<template>
  <div class="total-wrap">
    <div class="wrap mt-5">
      <img
        :src="require('@/assets/images/asnaf/esfahan-asnaf/line-magenta.png')"
        class="w-100"
      />
      <img
        :src="require('@/assets/images/asnaf/esfahan-asnaf/government-back.png')"
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
      font-family: 'B nazanin';
      color: white;
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
              font-family: 'Traffic';
            }
          }
          img {
            width: 120px;
            height: 70px;
          }
          .date {
            color: rgb(172, 172, 172);
            font-size: 12px;
            font-family: 'Traffic';
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
