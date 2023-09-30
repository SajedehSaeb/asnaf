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
    90deg,
    hsl(238deg 28% 65%) 0%,
    hsl(238deg 26% 62%) 11%,
    hsl(238deg 23% 59%) 22%,
    hsl(238deg 21% 57%) 33%,
    hsl(237deg 20% 54%) 44%,
    hsl(237deg 18% 51%) 56%,
    hsl(237deg 17% 49%) 67%,
    hsl(237deg 18% 46%) 78%,
    hsl(237deg 18% 44%) 89%,
    hsl(237deg 19% 41%) 100%
  );
  padding: 5px 10px;
  border-radius: 0 0 15px 15px;
}
</style>