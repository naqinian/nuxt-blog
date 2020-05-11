<template>
  <div class="about">
    <div class="t-container">
      <div class="my-left">
        <div class="my-adout">
          <div class="t-main-about">
            <div class="t-about-img">
              <img src="~/assets/img/2020462134088922.jpg" alt />
            </div>
            <div class="t-about-content">
              <p class="name">从前有个如初</p>
              <p class="address">中国&nbsp;|&nbsp;四川&nbsp;|&nbsp;成都</p>
              <p class="address">China&nbsp;|&nbsp;SiChuan&nbsp;|&nbsp;ChengDu</p>
            </div>
          </div>
        </div>
      </div>

      <div class="my-right">
       <div class="my">
    <div class="my-data">
      <i class="iconfont icon-icon_namecard_fill"></i>
      个人信息
    </div>
    <div class="my-about">
      <p>如初。</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;90后Web前端设计师、网页设计师。</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;出生于四川大山深处的某座小城市。</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;喜欢简约和一切美好的事情。</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;喜欢简简单单，喜欢平平淡淡。</p>
    </div>
    <div class="my-data">
      <i class="iconfont icon-icon_journal_fill"></i>
      个人技能
    </div>
    <div class="my-about">
      <p>前端：</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;1、熟悉html(5)、css(3)、javascript、jquery、bootstrap、layui、element-ui、vue(全家桶)、webpack、uniapp、mui...</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;2、了解WebSocket</p>
      <p>后端：</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;1、了解Golang</p>
      <p>数据库：</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;1、了解MYSQL数据库</p>
      <p>其他：</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;1、熟悉Git、IDEA、HBuider(X)、VSCode等开发工具</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;2、了解简单的PS操作</p>
    </div>
    <div class="my-data">
      <i class="iconfont icon-icon_addresslist_fil"></i>
      关于博客
    </div>
    <div class="my-about">
      <p>称&nbsp;&nbsp;&nbsp;号：如初。</p>
      <p>简&nbsp;&nbsp;&nbsp;介：好好学习，天天向上。</p>
      <p>大头图：xxxxxx</p>
      <p>域&nbsp;&nbsp;&nbsp;名：xxxxxxxx</p>
      <p>设&nbsp;&nbsp;&nbsp;计：如初。</p>
      <p>前&nbsp;&nbsp;&nbsp;端：nuxt、wangeditor3富文本</p>
      <p>后&nbsp;&nbsp;&nbsp;端：golang</p>
      <p>数据库：mysql</p>
      <p>服务器：阿里云</p>
      <p>备案号：xxxxxxx</p>
    </div>
    <div class="my-data">
      <i class="iconfont icon-icon_dmail_fill"></i>
      联系方式
    </div>
    <div class="my-about">
      <p>E-Mail：xxxxx@qq.com</p>
    </div>
  </div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.about {
  padding-top: 100px;
  padding-bottom: 60px;
  .t-container {
    border-radius: 8px;
    // padding: 40px 20px 20px 20px;
    .my-left {
      width: 25%;
      height: auto;
      float: left;
      display: block;
      padding-right: 20px;
      text-align: center;
      .my-adout {
        width: 100%;
        height: auto;
        background-color: #fff;
        border-radius: 8px;
        margin-bottom: 20px;
      }
      .t-main-about {
        padding: 20px;
      }
      .t-about-img {
        text-align: center;
        padding: 20px 0px;
      }
      .t-about-img img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
      }
      .t-about-content {
        padding: 20px 0px 10px 0px;
        text-align: center;
      }
      .t-about-content .name {
        font-size: 16px;
        padding-bottom: 4px;
      }
      .t-about-content .address {
        font-size: 12px;
      }
    }
    .my-right {
      width: 75%;
      height: auto;
      float: left;
      display: block;
      background-color: #fff;
    }
    .my {
      width: 100%;
      height: auto;
      padding: 20px 10px;
      border-radius: 8px;
      color: #405e79;
    }
    .my .my-data {
      width: 100%;
      height: 48px;
      font-size: 16px;
      padding: 13px 10px;
      border-bottom: 1px solid #e5e5e5;
    }
    .my .my-data img {
      width: 16px;
      height: 16px;
      margin-top: -2px;
      margin-right: 4px;
    }
    .my .my-about {
      width: 100%;
      height: auto;
      padding: 13px 10px;
      margin-bottom: 20px;
    }
    .my .my-about p {
      padding: 6px;
    }
  }
}
</style>