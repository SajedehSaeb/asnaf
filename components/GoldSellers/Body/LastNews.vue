<template>
  <div dir="rtl" >
    <div class="news-button">
      <b-button class="button">آخرین اخبار</b-button>
    </div>
    <div class="w-100 news mt-15">
      <b-row class="bg-white p-2 mt-3 last-news">
        <b-col
          v-for="(item, index) in news"
          :key="index"
          cols="12"
          lg="5"
          class="m-3 news-shadow"
        >
          <b-row>
            <b-col cols="10" lg="3">
              <b-img :src="item.image" class="image" />
            </b-col>
            <b-col cols="12" lg="9" class="news-title">
              {{ item.title }}
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      news: [
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/asnaf.png'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/person1.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
        {
          title: 'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت ',
          image: require('@/assets/goldSeller/sarami.jpg'),
        },
      ],
    }
  },
}
</script>

<style scoped>
.news-button {
  display: flex;
  justify-content: center;
  align-items: center;
}

.button {
  background-image: linear-gradient(90deg, #c9903f, #efe295);
  border-image: linear-gradient(90deg, #c9903f, #efe295);
  box-shadow: 5px 8px 5px rgba(128, 128, 128, 0.834);
  border-bottom-left-radius: 30px;
  border-bottom-right-radius: 30px;
  width: 65%;
  padding: 10px;
  font-family: 'Traffic';
  font-size: 25px;
  z-index: 1;
}

@media (min-width: 1440px) {
  .button {
    width: 16%;
  }
}

.news {
  display: flex;
  justify-content: center;
  align-items: center;
}

.last-news {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 70%;
  z-index: 1;
}

.image {
  width: 100%;
  height: 70px;
}
.news-title {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: end;
  font-family: 'Traffic';
}

.news-shadow{
  box-shadow: 2px 5px 8px rgb(158, 158, 158);
}
</style>
