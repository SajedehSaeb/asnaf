<template>
  <div class="wrap">
    <b-row>
      <b-col cols="12" lg="8" md="12"  sm="12">
       <div class="wrap-content">
        <img
          :src="require('@/assets/images/asnaf/socials.png')"
          alt="socials"
        />
        <RightHeaderSlider />
       </div>
      </b-col>
      <b-col cols="12" lg="4" md="12" sm="12">
        <LeftHeaderSlider />
        <HeaderOptions />
      </b-col>
    </b-row>
  </div>
</template>

<script>
import RightHeaderSlider from '@/components/asnaf/header/RightHeaderSlider.vue'
import LeftHeaderSlider from '@/components/asnaf/header/LeftHeaderSlider.vue'
import HeaderOptions from '@/components/asnaf/header/HeaderOptions.vue'
export default {
  name: 'HeaderBottom',
  components: {
    RightHeaderSlider,
    LeftHeaderSlider,
    HeaderOptions,
  },
}
</script>

<style scoped lang="scss">
.wrap {
  width: 85%;
  margin: 0 auto;
  &-content{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>