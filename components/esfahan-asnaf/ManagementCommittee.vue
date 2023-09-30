<template>
  <div class="wrap">
    <img
      :src="require('@/assets/images/asnaf/esfahan-asnaf/commite-back.png')"
      class="back1"
    />
    <div class="caption">
      <img
        :src="require('@/assets/images/asnaf/esfahan-asnaf/line-magenta.png')"
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
    @media screen and (max-width: 992px) {
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
      font-family: 'B nazanin';
      font-size: 25px;
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
            font-family: 'Traffic';
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
      font-size: 22px;
      border: none;
      padding: 10px 25px;
      border-radius: 10px;
      font-family: 'B nazanin';
    }
  }
}
</style>
