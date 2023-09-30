<template>
  <div class="wrap">
    <img
      :src="require('@/assets/images/asnaf/tehran-asnaf/commite-back.png')"
      class="back1"
    />
    <div class="caption">
      <img
        :src="require('@/assets/images/asnaf/tehran-asnaf/line-magenta.png')"
        class="w-100"
      />
      <span class="title d-flex justify-content-center align-items-center">
        هیئت رئیسه
      </span>
    </div>
    <div class="wrap-content">
      <div class="items d-flex flex-wrap justify-content-between">
        <div
          v-for="(item, index) in category"
          :key="index"
          class="mt-2 wrap-single rounded-pill d-flex align-items-center flex-wrap"
        >
          <div class="single d-flex align-items-center">
            <div class="wrap-img">
              <img
                :src="require('@/assets/images/asnaf/news/1.jpg')"
                alt="news"
              />
            </div>
            <div class="px-2 py-2">
              <p class="description">{{ item.content }}</p>
            </div>
          </div>
        </div>
      </div>
      <div class="d-flex justify-content-center my-4">
        <button class="union-btn">اتحادیه ها</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ManagementCommittee',
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
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.wrap {
  position: relative;
  .back1 {
    position: absolute;
    left: 8%;
    @media screen and (max-width:992px) {
      display: none;
    }
  }
  .caption {
    width: 60%;
    margin: 0 auto;
    position: relative;
    display: flex;
    justify-content: center;
    .title {
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
      color: white;
      font-family: 'B nazanin';
      font-size: 22px;
      position: absolute;
      top: 55%;
      border-radius: 0 0 30px 30px;
      width: 200px;
      padding: 13px 40px;
      -webkit-box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
      -moz-box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
      box-shadow: 8px 11px 7px 0px rgba(179, 170, 179, 1);
    }
  }
  &-content {
    width: 60%;
    margin: 0 auto;
    margin-top: 80px;
    .items {
      .wrap-single {
        width: 30%;
        &:nth-child(1) {
          background-color: #f2f2f2;
          padding: 10px;
        }
        @media screen and (max-width: 1200px) {
          width: 48%;
        }
        @media screen and (max-width: 992px) {
          width: 100%;
          border-radius: 15px !important;
        }
        .single {
          width: 100%;
          text-align: right;
          @media screen and (max-width: 578px) {
            flex-direction: column;
          }
          .description {
            font-size: 12px;
          }
          .wrap-img {
            width: 350px;
            height: 100px;
            border-radius: 50%;
            @media screen and (max-width: 992px) {
              width: 150px;
              height: 100px;
            }
            @media screen and (max-width: 768px) {
              width: 250px;
              height: 100px;
            }
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
        }
      }
    }
    .union-btn {
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
      color: white;
      font-family: 'B nazanin';
      font-size: 25px;
      border: none;
      padding: 10px 25px;
      border-radius: 10px;
    }
  }
}
</style>
