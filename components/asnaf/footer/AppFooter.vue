<template>
  <div class="wrapper">
    <img :src="require('@/assets/images/asnaf/gear.png')" class="gear" />
    <img
      :src="require('@/assets/images/asnaf/footer/footer-back.png')"
      class="back"
    />
    <div class="footer d-flex flex-wrap">
      <div class="single">
        <SocialNetworks />
      </div>
      <div class="single">
        <QuickAccess />
      </div>
      <div class="single">
        <RelatedLinks />
      </div>
      <div class="single">
        <FooterAddress />
      </div>
    </div>
  </div>
</template>

<script>
import SocialNetworks from '@/components/asnaf/footer/SocialNetworks.vue'
import QuickAccess from '@/components/asnaf/footer/QuickAccess.vue'
import RelatedLinks from '@/components/asnaf/footer/RelatedLinks.vue'
import FooterAddress from '@/components/asnaf/footer/FooterAddress.vue'
export default {
  name: 'AppFooter',
  components: {
    SocialNetworks,
    QuickAccess,
    RelatedLinks,
    FooterAddress,
  },
}
</script>

<style scoped lang="scss">
.wrapper {
  background-color: #6d6e71;
  color: white;
  padding: 15px 0;
  -webkit-box-shadow: inset 0px 6px 19px -3px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: inset 0px 6px 19px -3px rgba(0, 0, 0, 0.75);
  box-shadow: inset 0px 6px 19px -3px rgba(0, 0, 0, 0.75);
  position: relative;
  overflow: hidden;

  .back {
    position: absolute;
    left: 0;
    bottom: 0;
    height: 100%;
    z-index: 1;
    @media screen and (max-width:768px) {
      display: none;
    }
  }
  .gear {
    position: absolute;
    right: 63%;
    z-index: 1;
    top: -15%;
  }
  .footer {
    width: 70%;
    margin: 0 auto;
    .single {
      width: 25%;
      @media screen and (max-width:992px) {
        width: 50%;
      }
      @media screen and (max-width:578px) {
        width: 100%;
      }
    }
  }
}
</style>