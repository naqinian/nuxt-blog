<template>
  <div class="load">
    <div class="load-up" @click="getTop()">
      <img src="~/assets/img/load.png" alt />
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  methods: {
    // 动态监听
    handleScroll() {
      let bodyTop =
        document.body.scrollTop || document.documentElement.scrollTop;
      let loadCSS = document.getElementsByClassName("load-up")[0];
      if (bodyTop >= 100) {
        loadCSS.style.cssText = "transition:.4s;opacity:1;right:30px;";
      } else {
        loadCSS.style.cssText = "transition:.4s;opacity:0;right:-100px";
      }
    },
    // 返回置顶
    getTop() {
      let top = document.documentElement.scrollTop || document.body.scrollTop;
      // 实现滚动效果
      const timeTop = setInterval(() => {
        document.body.scrollTop = document.documentElement.scrollTop = top -= 100;
        if (top <= 0) {
          clearInterval(timeTop);
        }
      }, 20);
    }
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  }
};
</script>

<style scoped>
.load{position:fixed;bottom:100px;right:30px;z-index:1000;width:40px;height:auto;padding:4px;}.load-up{background-color:#33cb98;color:#fff;border-radius:4px;position:fixed;width:40px;height:40px;padding:10px;right:-100px;opacity:0;}.load-up img{width:100%;height:100%;}.load::after{content:"";display:table;clear:both;}
</style>