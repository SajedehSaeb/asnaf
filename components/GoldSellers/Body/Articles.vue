<template>
  <div class="d-flex justify-content-center align-item-center mt-3" dir="rtl">
    <b-row class="w-75">
      <b-col cols="12" lg="6" xl="4">
        <b-row>
          <b-col
            cols="12"
            class="d-flex justify-content-center align-item-center"
          >
            <b-button class="article-button">مقالات</b-button>
          </b-col>
          <b-col
            cols="12"
            class="report-title"
          >
            <b-row class="w-75 mt-3">
              <p>لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله در ستون و سطرآنچنان که </p>
            </b-row>
          </b-col>
        </b-row>
      </b-col>

      <b-col cols="12" lg="6" xl="4">
        <b-row>
          <b-col
            cols="12"
            class="d-flex justify-content-center align-item-center"
          >
            <b-button class="article-button">گزارش</b-button>
          </b-col>
          <b-col
            cols="12"
            class="d-flex justify-content-center align-item-center"
          >
            <b-row class="w-100 mt-3">
              <b-col
                v-for="(item, index) in reports"
                :key="index"
                cols="12"
                class="m-2 report-bg"
              >
                <b-row>
                  <b-col cols="3" class="report-img">
                    <b-img :src="item.image" class="image" />
                  </b-col>
                  <b-col cols="9" class="report-title">
                    {{ item.title }}
                  </b-col>
                </b-row>
              </b-col>
            </b-row>
          </b-col>
        </b-row>
      </b-col>

      <b-col cols="12" lg="6" xl="4">
        <b-row>
          <b-col
            cols="12"
            class="d-flex justify-content-center align-item-center"
          >
            <b-button class="article-button">پربازدیدترین ها</b-button>
          </b-col>
          <b-col
            cols="12"
            class="d-flex justify-content-center align-item-center"
          >
            <b-row class="w-100 mt-3">
              <b-col
                v-for="(item, index) in reports"
                :key="index"
                cols="12"
                class="m-2 report-bg"
              >
                <b-row>
                  <b-col cols="3" class="report-img">
                    <b-img :src="item.image" class="image" />
                  </b-col>
                  <b-col cols="9" class="report-title">
                    {{ item.title }}
                  </b-col>
                </b-row>
              </b-col>
            </b-row>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      reports: [
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/person1.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/person1.jpg'),
        },
      ],
    }
  },
}
</script>

<style scoped>
.article-button {
  background-image: linear-gradient(90deg, #c9903f, #efe295);
  border-image: linear-gradient(90deg, #c9903f, #efe295);
  width: 50%;
  border-radius: 35px;
  font-family: 'Traffic';
  font-weight: bold;
}

@media (max-width: 425px){
  .article-button{
    width: 75%;
  }
}

.image {
  width: 130%;
  height: 70px;
}

.report-bg {
  background-color: #f2f2f2;
}

.report-img {
  display: flex;
  justify-content: start;
  align-items: start;
}

.report-title {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: end;
  font-family: 'Traffic';
}
</style>
