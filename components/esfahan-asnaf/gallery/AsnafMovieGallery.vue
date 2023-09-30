<template>
  <div class="total-wrap mt-5">
    <img
      :src="require('@/assets/images/asnaf/tehran-asnaf/gallery-back.png')"
      class="back1"
    />
    <img
      :src="require('@/assets/images/asnaf/tehran-asnaf/gallery-back2.png')"
      class="back2"
    />
    <div class="wrap-gallery">
      <div class="caption">
        <img
          :src="require('@/assets/images/asnaf/tehran-asnaf/line-magenta.png')"
          class="w-100"
        />
        <span
          class="title d-flex justify-content-center align-items-center text-center"
        >
          گالری فیلم و عکس
        </span>
      </div>
      <div class="wrap-content">
        <div>
          <b-row class="justify-content-between">
            <b-col cols="12" lg="5">
              <RightGallery />
            </b-col>
            <b-col cols="12" lg="5">
              <LeftGallery />
            </b-col>
          </b-row>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import RightGallery from '~/components/esfahan-asnaf/gallery/RightGallery'
import LeftGallery from '~/components/esfahan-asnaf/gallery/LeftGallery'
export default {
  name: 'AsnafMovieGallery',
  components: { RightGallery, LeftGallery },
}
</script>

<style scoped lang="scss">
.total-wrap {
  overflow: hidden;
  position: relative;
  padding-bottom: 100px;
  background-image: linear-gradient(
  0deg,
  hsl(182deg 84% 41%) 0%,
  hsl(183deg 52% 53%) 11%,
  hsl(183deg 50% 60%) 22%,
  hsl(183deg 49% 67%) 33%,
  hsl(183deg 48% 73%) 44%,
  hsl(183deg 47% 78%) 56%,
  hsl(183deg 47% 84%) 67%,
  hsl(182deg 46% 89%) 78%,
  hsl(182deg 46% 95%) 89%,
  hsl(0deg 0% 100%) 100%
);
  .back1 {
    position: absolute;
    left: 5%;
    bottom: 0;
  }
  .back2 {
    position: absolute;
    right: 0.5%;
    bottom: 10%;
  }
  .wrap-gallery {
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
    .wrap-content {
      margin-top: 100px;
    }
  }
}
</style>
