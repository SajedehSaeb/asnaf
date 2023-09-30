<template>
  <div class="wrap-gallery">
    <img
      :src="require('@/assets/images/asnaf/gallery-back2.png')"
      class="right-back"
    />
    <img
      :src="require('@/assets/images/asnaf/gallery-back.png')"
      class="left-back"
    />
    <div class="wrap-content mt-3">
      <div class="head">
        <HeaderCaption title="گالری فیلم و عکس" />
      </div>
      <div class="wrap-content-slider">
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
</template>

<script>
import HeaderCaption from '~/components/asnaf/common/HeaderCaption.vue'
import RightGallery from '~/components/asnaf/gallery/RightGallery'
import LeftGallery from '~/components/asnaf/gallery/LeftGallery'
export default {
  name: 'MovieGallery',
  components: { HeaderCaption, RightGallery, LeftGallery },
}
</script>

<style scoped lang="scss">
.wrap-gallery {
  overflow: hidden;
  position: relative;
  padding-bottom: 100px;
  background-image: linear-gradient(
    0deg,
    hsl(207deg 74% 42%) 0%,
    hsl(211deg 51% 52%) 11%,
    hsl(213deg 50% 59%) 22%,
    hsl(215deg 49% 66%) 33%,
    hsl(216deg 49% 72%) 44%,
    hsl(217deg 49% 77%) 56%,
    hsl(218deg 49% 83%) 67%,
    hsl(219deg 49% 89%) 78%,
    hsl(219deg 49% 94%) 89%,
    hsl(0deg 0% 100%) 100%
  );
  .wrap-content {
    width: 70%;
    margin: 0 auto;
    &-slider{
           margin-top: 120px;


    }
    font-family: 'B nazanin';
  }
  .right-back {
    position: absolute;
    right: 0;
    bottom: -24%;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
  .left-back {
    position: absolute;
    left: 0;
    top: 7%;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
}
</style>
