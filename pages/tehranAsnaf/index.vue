<template>
  <div>
    <MainHeader />
    <AsnafServices />
    <ManagementCommittee />
    <AsnafLastNews />
    <MarketNews />
    <AsnafMovieGallery />
    <ActivityDiscussion />
    <AsnafGovernment />
    <FooterApp />
  </div>
</template>

<script>
import MainHeader from '@/components/tehran-asnaf/header/MainHeader.vue'
import AsnafServices from '@/components/tehran-asnaf/services/AsnafServices.vue'
import ManagementCommittee from '@/components/tehran-asnaf/ManagementCommittee.vue'
import AsnafLastNews from '@/components/tehran-asnaf/AsnafLastNews.vue'
import MarketNews from '@/components/tehran-asnaf/MarketNews.vue'
import ActivityDiscussion from '@/components/tehran-asnaf/ActivityDiscussion.vue'
import AsnafGovernment from '@/components/tehran-asnaf/AsnafGovernment.vue'
import FooterApp from '@/components/tehran-asnaf/FooterApp.vue'
import AsnafMovieGallery from '@/components/tehran-asnaf/gallery/AsnafMovieGallery.vue'
export default {
  name: 'indexPage',
  components: {
    MainHeader,
    AsnafServices,
    ManagementCommittee,
    AsnafLastNews,
    MarketNews,
    AsnafMovieGallery,
    ActivityDiscussion,
    AsnafGovernment,
    FooterApp,
  },
}
</script>

<style scoped lang="scss">
</style>