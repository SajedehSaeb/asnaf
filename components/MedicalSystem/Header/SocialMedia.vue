<template>
  <div class="social-media">
    <b-row class=" media">

      <!-- <b-img src="@/assets/goldSeller/eta.png" class="mx-1" /> -->

      <b-img src="@/assets/goldSeller/Asset 48.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 45.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 44.png" class="mx-1" />
      <b-img src="@/assets/goldSeller/Asset 43.png" class="mx-1" />
      <b-img src="@/assets/medical/email.png" class="mx-1" />

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
  background-color: #662d91;
  padding: 10px;
  width: 13vw;
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
    width: 13%;
  }
}

.media {
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
