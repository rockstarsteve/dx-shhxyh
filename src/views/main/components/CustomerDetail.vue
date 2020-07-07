<template>
    <div class="customer-detail">
        <div class="title">客户详情</div>
        <div class="content">
            <div class="left">
                <img :src="userImg" class="user-img" alt="">
            </div>
            <div class="right">
                <div class="right-title">业务开办种类：</div>
            </div>
        </div>
    </div>
</template>

<script>
  export default {
    name: "ConsumerDetail",
    data() {
      return {
        userImg: require('assets/images/main/user.jpg'),
      }
    }
  }
</script>

<style lang="less" scoped>
    .customer-detail {
        width: 948rem;

        .title {
            font-family: PingFang;
            font-size: 22rem;
            font-weight: 600;
            line-height: 30rem;
            color: rgba(70, 65, 65, 1);
        }

        .content {
            margin-top: 30rem;
            width: 948rem;
            height: 260rem;
            background: #FAFAFA;
            border-radius: 20rem;
            display: flex;

            .left {
                width: 500rem;
                padding-left: 20rem;
                padding-top: 25rem;
                .user-img{
                    width: 60rem;
                    height: 60rem;
                    border-radius: 50%;
                }
            }

            .right {

            }
        }

    }

</style>
