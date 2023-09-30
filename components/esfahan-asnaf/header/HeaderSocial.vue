<template>
  <div class="wrap-socials d-flex justify-content-center align-items-center">
    <div>
      <i
        v-for="(icon, index) in icons"
        :key="index"
        :class="icon.title"
        class="mx-2"
      ></i>
    </div>
    <img
      class="mx-2"
      :src="require('@/assets/images/asnaf/tehran-asnaf/eta.png')"
    />
    <i class="icon-house mx-2"></i>
  </div>
</template>

<script>
export default {
  name: 'HeaderSocial',
  data() {
    return {
      icons: [
        { title: 'icon-twitter' },
        { title: 'icon-facebook' },
        { title: 'icon-instagram' },
        { title: 'icon-youtube' },
      ],
    }
  },
}
</script>

<style scoped lang="scss">
.wrap-socials {
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
  padding: 10px 15px;
  border-radius: 0 0 15px 15px;
  i {
    font-size: 20px;
  }
}
</style>