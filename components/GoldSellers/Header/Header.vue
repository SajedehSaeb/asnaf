
<template>
  <div class="heder">
    <div>
      <b-img src="@/assets/goldSeller/HeaderGold.jpg" class="image" />
    </div>
    <div class="heder-filter"></div>
    <div class="diamond">
      <b-img src="@/assets/goldSeller/Asset 53.png" class="logo-image" />
    </div>
    <div class="header1">
      <b-img src="@/assets/goldSeller/Asset 52.png" />
    </div>
    <div class="header2">
      <b-img src="@/assets/goldSeller/Asset 51.png" />
    </div>
    <div class="line">
      <b-img src="@/assets/goldSeller/line.png" />
    </div>
    <div class="logo">
      <b-img src="@/assets/goldSeller/logoTala.png" class="logo-image" />
    </div>
    <div class="titr">
      <div class="titr-senf">
        <h2>اتحادیه صنف فروشندگان و سازندگان طلا،جواهر،نقره و سکه تهران</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent',
}
</script>

<style scoped>
.heder {
  position: relative;
  /* height: 30vh; */
  /* width: 100%; */
}

.image {
  width: 100%;
  height: 30vh;
}

.logo {
  position: absolute;
  top: 10%;
  left: 45%;
}

.titr-senf {
  position: absolute;
  top: 70%;
  font-family: 'IranNastaliq';
  color: #a5794c;
}
.titr {
  display: flex;
  justify-content: center;
  align-items: center;
  /* left: 45%; */
}
.heder-filter {
  position: absolute;
  background-color: #f6ebdb96;
  top: 0;
  width: 100%;
  height: 100%;
}

h2 {
  font-size: 50px;
}

.diamond {
  position: absolute;
  bottom: 0;
  left: 1%;
}

.line {
  position: absolute;
  bottom: 0;
  left: 0;
}

.header1 {
  position: absolute;
  top: 0;
  left: 25%;
}

.header2 {
  position: absolute;
  bottom: 0;
  right: 3%;
}

@media (max-width: 768px) {
  h2 {
    font-size: 25px;
  }
  .logo-image {
    width: 70%;
  }

  .logo {
    position: absolute;
    top: 10%;
    left: 40%;
  }
  .diamond {
    position: absolute;
    bottom: 0;
    left: 3%;
  }
}

/* @media () {
  h2 {
    font-size:30px;
  }

  .logo-image {
    width: 65%;
  }
} */
</style>
