<template>
  <div>
    <MainHeader />
    <Services />
    <LastNews />
    <ReportImage />
    <AsnafNews />
    <BoardNews />
    <ReportVisitor />
    <TopPublicRelationship />
    <AsnafProvince />
    <MovieGallery />
    <FooterServices />
    <AppFooter />
  </div>
</template>

<script>
import MainHeader from '~/components/asnaf/header/MainHeader'
import Services from '@/components/asnaf/services/Services'
import LastNews from '@/components/asnaf/news/LastNews'
import ReportImage from '@/components/asnaf/reportImage/ReportImage'
import AsnafNews from '@/components/asnaf/news/AsnafNews'
import BoardNews from '@/components/asnaf/news/BoardNews'
import ReportVisitor from '@/components/asnaf/reportImage/ReportVisitor'
import TopPublicRelationship from '@/components/asnaf/reportImage/TopPublicRelationship'
import AsnafProvince from '@/components/asnaf/AsnafProvince'
import MovieGallery from '@/components/asnaf/gallery/MovieGallery'
import FooterServices from '@/components/asnaf/footer/FooterServices'
import AppFooter from '@/components/asnaf/footer/AppFooter'
export default {
  name: 'IndexPage',
  components: {
    MainHeader,
    Services,
    LastNews,
    ReportImage,
    AsnafNews,
    BoardNews,
    ReportVisitor,
    TopPublicRelationship,
    AsnafProvince,
    MovieGallery,
    FooterServices,
    AppFooter,
  },
}
</script>

<style scoped lang="scss">
</style>
