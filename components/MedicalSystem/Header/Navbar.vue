<template>
  <div dir="rtl">
    <b-navbar toggleable="lg" type="dark">
      <b-navbar-brand href="#">
        <b-img src="@/assets/medical/Asset 21.png" />
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse">
        <i class="icon-menu"></i>
      </b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav class="">
        <b-navbar-nav>
          <b-nav-item href="#">صفحه اصلی</b-nav-item>
          <b-nav-item href="#">درباره ما </b-nav-item>
          <b-nav-item href="#">اطلاع رسانی</b-nav-item>
          <b-nav-item href="#">اخبار</b-nav-item>
          <b-nav-item href="#">مرکز دانش</b-nav-item>
          <b-nav-item href="#">ارتباط با ما</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-button class="user-login">ورود اعضا</b-button>
          </b-nav-form>
        </b-navbar-nav>

        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <div
              class="search d-flex justify-content-center align-items-center py-2 mt-2"
            >
              <b-row class="w-100 h-75">
                <b-col
                  cols="2"
                  class="d-flex justify-content-center align-items-center text-white font-style"
                >
                  جستجو
                </b-col>
                <b-col cols="8" class="w-100 h-100 bg-white">
                  <b-form-input
                    id="input-1"
                    type="text"
                    class="w-100"
                  ></b-form-input>
                </b-col>
                <b-col
                  cols="2"
                  class="d-flex justify-content-center align-items-center search-font"
                >
                  <b-img src="@/assets/medical/search.png" class="mx-1" />
                </b-col>
              </b-row>
            </div>
          </b-nav-form>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
  <!-- <div class="py-2">
    <b-row class="w-100">
      <b-col
        cols="6"
        md="3"
        class="d-none d-md-flex justify-content-end align-items-center"
      >
        <b-row class="search w-75 py-2 px-3 d-flex justify-content-center align-items-center">
          <b-col class="d-flex justify-content-center align-items-center">
          </b-col>
          <b-col cols="6" class="w-100 h-100 bg-white py-3">
          </b-col>
          <b-col class="d-flex justify-content-center align-items-center search-font">
            جستجو
          </b-col>
        </b-row>
      </b-col>
      <b-col
        cols="6"
        md="1"
        class="d-none d-md-flex justify-content-end align-items-center"
      >
        <b-button class="user-login">ورود اعضا</b-button>
      </b-col>

      <b-col
        cols="7"
        md="6"
        class="d-none d-md-flex justify-content-end align-items-center"
      >
        <div>
          <a href="#">صفحه اصلی</a>
          <a href="#">درباره ما </a>
          <a href="#">اطلاع رسانی</a>
          <a href="#">اخبار</a>
          <a href="#">مرکز دانش</a>
          <a href="#">ارتباط با ما</a>
        </div>
      </b-col>
      <b-col
        cols="6"
        md="2"
        class="d-flex justify-content-center align-items-center"
      >
        <b-img src="@/assets/medical/Asset 21.png" />
      </b-col>
      <b-col cols="6" class="d-flex d-md-none justify-content-end align-items-center">
        <i class="icon-menu"></i>
      </b-col>
    </b-row>
  </div> -->
</template>

<script>
export default {}
</script>

<style scoped>
.form-control {
  border: 1px solid white;
}

.form-control:focus {
  outline: none !important;
  border: none !important;
}
.navbar-dark .navbar-nav .nav-link {
  font-family: 'B nazanin';
  color: #662d91;
  font-size: 25px;
}

.search {
  background-color: #662d91;
  border-radius: 15px;
  width: 25vw;
  /* height: 20vh; */
}

@media (max-width: 768px) {
  .search {
    width: 80vw;
  }
}

.user-login {
  background-color: rgb(236, 236, 236);
  border: 1px solid rgb(219, 219, 219);
  border-radius: 0%;
  color: #662d91;
  font-family: 'B nazanin';
  box-shadow: 1px 2px 5px grey;
}

.font-style {
  font-family: 'B nazanin';
}

.icon-menu {
  font-size: 25px;
  color: rgb(59, 59, 59) !important;
}
/* a {
  font-family: 'B nazanin';
  color: #662d91;
  font-size: 25px;
  margin: 20px;
}

.search-font {
  font-family: 'B nazanin';
  font-weight: bold;
  color: white;
}





 */
</style>
