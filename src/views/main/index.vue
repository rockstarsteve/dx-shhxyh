<template>
    <div class="container">
        <div class="left">
            <img :src="logoImg" class="logo-img" alt="">
            <customer-detail></customer-detail>

        </div>
        <div class="right">

        </div>
    </div>
</template>

<script>
  import CustomerDetail from './components/CustomerDetail'

  export default {
    name: "index",
    components: {
      CustomerDetail
    },
    data() {
      return {
        logoImg: require('assets/images/login/logo.png'),

      }
    }
  }
</script>

<style lang="less" scoped>
    .container {
        height: 100vh;
        background: rgba(250, 250, 250, 1);
        position: relative;

        .left {
            width: 1140rem;
            height: 100%;
            box-shadow: 8rem 2rem 61rem 0rem rgba(0, 0, 0, 0.04);
            position: relative;
            padding-top: 148rem;
            padding-left: 100rem;
            background: rgba(255, 255, 255, 1);

            .logo-img {
                width: 130rem;
                height: 50rem;
                position: absolute;
                top: 34rem;
                left: 70rem;
            }
        }

        .right {
            width: 780rem;
            height: 100%;
            background: rgba(250, 250, 250, 1);
        }
    }
</style>
