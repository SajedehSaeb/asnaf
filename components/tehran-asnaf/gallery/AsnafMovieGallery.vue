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
import RightGallery from '~/components/tehran-asnaf/gallery/RightGallery'
import LeftGallery from '~/components/tehran-asnaf/gallery/LeftGallery'
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
    180deg,
    hsl(0deg 0% 100%) 0%,
    hsl(273deg 26% 93%) 11%,
    hsl(273deg 25% 86%) 22%,
    hsl(273deg 24% 79%) 33%,
    hsl(273deg 23% 73%) 44%,
    hsl(273deg 21% 66%) 56%,
    hsl(273deg 20% 60%) 67%,
    hsl(273deg 19% 54%) 78%,
    hsl(273deg 19% 48%) 89%,
    hsl(273deg 21% 43%) 100%
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
