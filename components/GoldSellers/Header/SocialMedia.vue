<template>
  <div class="social-media">
    <b-row class="w-100 media">
      <b-img src="@/assets/goldSeller/Asset 46.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/eta.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 43.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 44.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 45.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 48.png" class="mx-1" />
    </b-row>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.social-media {
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
  background-image: linear-gradient(#efe295, #c9903f);
  border-image: linear-gradient(#efe295, #c9903f);
  width: 16%;
  padding: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
}



@media (width: 768px) {
  .social-media {
    width: 40%;
  }
}

@media (max-width: 425px) {
  .social-media {
    width: 60%;
  }
}

@media (min-width: 1024px) {
  .social-media {
    width: 30%;
  }
}

@media (min-width: 1440px) {
  .social-media {
    width: 20%;
  }
}

.media {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
