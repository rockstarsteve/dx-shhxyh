<template>
    <transition name="fade">
        <div class="toast" v-show="show">
            {{message}}
        </div>
    </transition>
</template>

<script>
  export default {
    data() {
      return {
        show: false,
        message: ""
      };
    }
  };
</script>

<style lang="less" scoped>
    .toast {
        position: fixed;
        top: 40%;
        left: 50%;
        margin-left: -7vw;
        padding: 1vw;
        width: 15vw;
        font-size: 1vw;
        color: #fff;
        text-align: center;
        background-color: rgba(0, 0, 0, 0.8);
        border-radius: 1vw;
        z-index: 999;
    }

    .fade-enter-active,
    .fade-leave-active {
        transition: 0.3s ease-out;
    }

    .fade-enter {
        opacity: 0;
        transform: scale(1.2);
    }

    .fade-leave-to {
        opacity: 0;
        transform: scale(0.8);
    }
</style>
