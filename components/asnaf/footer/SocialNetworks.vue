<template>
  <div class="wrap">
    <div class="content d-flex flex-column">
      <strong class="caption">شبکه های اجتماعی</strong>
      <div class="socials mt-2">
        <div v-for="(item, index) in socials" :key="index" class="d-flex mt-2">
          <i :class="[item.icon, item.class]"></i>
          <h6 class="mr-2">{{ item.title }}</h6>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SocialNetworks',
  data() {
    return {
      socials: [
        {
          title: 'عضویت در کانال تلگرام',
          icon: 'icon-telegram',
        },
        { title: 'عضویت در اینستاگرام', icon: 'icon-instagram' },
        {
          title: 'مارادرتوییتردنبال کنید',
          icon: 'icon-twitter',
          class: '00AEEF',
        },
        { title: 'مارادر فیسبوک دنبال کنید', icon: 'icon-facebook' },
      ],
    }
  },
}
</script>

<style lang="scss" scoped >
.wrap {
  .content {
    .caption {
      font-size: 27px;
      text-align: right;
      font-family: 'B nazanin';
    }
    .socials {
      font-family: 'B nazanin';
      .icon-telegram::before {
        color: #27aae1 !important;
      }
      .icon-instagram::before {
        background: radial-gradient(
          circle at 30% 107%,
          #fdf497 0%,
          #fdf497 5%,
          #fd5949 45%,
          #d6249f 60%,
          #285aeb 90%
        );
        -webkit-background-clip: text;
        background-clip: text;
        -webkit-text-fill-color: transparent;
      }
      .icon-twitter::before {
        color: #27aae1 !important;
      }
      .icon-facebook::before {
        color: #2b3990 !important;
      }

      h6 {
        font-size: 12px;
        text-align: right;
      }
    }
  }
}
</style>
