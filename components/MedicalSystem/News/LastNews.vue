<template>
  <div class="last-news-style">
    <b-row class="w-100">
      <b-col cols="12" v-for="(item, index) in news" :key="index" class="m-2">
        <b-row>
          <b-col cols="9" class="text-right">
            <p>{{ item.title }}</p>
          </b-col>
          <b-col cols="3">
            <b-img :src="item.image" class="image" />
          </b-col>
        </b-row>
      </b-col>
    </b-row>
    <b-row class="d-flex justify-content-center align-item-center">
      <b-button class="btn-style px-3">
        <b-img src="@/assets/medical/Asset 33.png" />
        آرشیو
      </b-button>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      news: [
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        {
          title:
            'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
          image: require('@/assets/goldSeller/person2.jpg'),
        },
        // {
        //   title:
        //     'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
        //   image: require('@/assets/goldSeller/person2.jpg'),
        // },
        // {
        //   title:
        //     'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
        //   image: require('@/assets/goldSeller/person2.jpg'),
        // },
        // {
        //   title:
        //     'لورم ایپسوم متن ساختگی با تولید سادگی نامفهوم از صنعت چاپ، و با استفاده از طراحان گرافیک است، چاپگرها و متون بلکه روزنامه و مجله ',
        //   image: require('@/assets/goldSeller/person2.jpg'),
        // },
      ],
    }
  },
}
</script>

<style scoped>
.last-news-style {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
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
}

.news-title {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: end;
  font-family: 'Traffic';
}

.image {
  width: 100%;
  height: 70px;
}

p {
  font-family: 'B nazanin';
  font-weight: bold;
  font-size: 15px;
}

p:hover {
  color: green;
  cursor: pointer;
}

.btn-style {
  background-color: #a01f62;
  border-color: #a01f62;
  border-radius: 10px;
}
</style>
