<template>
  <div>
    <!-- 导航栏 -->
    <app-header />
    <!-- 内容 -->
    <nuxt />
    <!-- 返回置顶 -->
    <app-load />
    <!-- 底部版权 -->
    <app-footer />
  </div>
</template>

<script>
import Header from "~/components/Header";
import Footer from "~/components/Footer";
import Load from "~/components/Load";

export default {
  components: {
    "app-header": Header,
    "app-footer": Footer,
    "app-load": Load
  }
};
</script>

