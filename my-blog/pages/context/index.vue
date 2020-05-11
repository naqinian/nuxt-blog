<template>
  <div class="content">
    <div class="t-container">
      <div class="content-title">文章标题</div>
      <div class="content-other">
        <i class="iconfont icon-time"></i>
        发布时间&nbsp;
        <i class="iconfont icon-yueduxiao"></i>
        阅读量
      </div>
      <div class="content-txt">
        <div>文章内容</div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.content {
  padding-top: 100px;
  padding-bottom: 60px;
  .t-container {
    background-color: #fff;
    border-radius: 8px;
    padding-top: 40px;
    padding-bottom: 20px;
  }
  .content-title {
    font-size: 20px;
    text-align: center;
    padding: 6px 0;
  }
  .content-other {
    font-size: 14px;
    padding: 10px 0px;
    border-bottom: 1px dashed #eee;
    text-align: center;
  }
  .content-txt {
    padding: 10px 20px;
    width: 100%;
    height: auto;
  }
  .content-txt pre {
    background-color: #929292;
    border-radius: 6px;
    width: 100%;
    height: auto;
  }
}
</style>