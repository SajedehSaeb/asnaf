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
  import MainHeader from '@/components/esfahan-asnaf/header/MainHeader.vue'
  import AsnafServices from '@/components/esfahan-asnaf/services/AsnafServices.vue'
  import ManagementCommittee from '@/components/esfahan-asnaf/ManagementCommittee.vue'
  import AsnafLastNews from '@/components/esfahan-asnaf/AsnafLastNews.vue'
  import MarketNews from '@/components/esfahan-asnaf/MarketNews.vue'
  import ActivityDiscussion from '@/components/esfahan-asnaf/ActivityDiscussion.vue'
  import AsnafGovernment from '@/components/esfahan-asnaf/AsnafGovernment.vue'
  import FooterApp from '@/components/esfahan-asnaf/FooterApp.vue'
  import AsnafMovieGallery from '@/components/esfahan-asnaf/gallery/AsnafMovieGallery.vue'
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