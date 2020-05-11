<template>
  <div class="book">
    <div class="t-container">
      <div class="book-right">
        <div class="article-ul">
          <div class="article-li">
            <nuxt-link :to="{name:'context'}">
            <div
              class="article-con"
              style="background-image:url(https://i.loli.net/2020/01/31/Tp3bE5FCeBNAjSI.jpg)"
            >
              <div class="article-cc"></div>
              <div class="article">
                <div class="article-title">文章标题</div>
                <div class="article-txt">文章简介</div>
                <div class="article-qt">
                  <i class="iconfont icon-browse"></i>
                  点击量：&nbsp;
                  <i class="iconfont icon-time"></i>
                  发布时间：
                </div>
              </div>
            </div>
            </nuxt-link>
          </div>
          <div class="article-li">
            <!-- <nuxt-link :to="{name:'content' ,query:{id:book.id}}"> -->
            <div
              class="article-con"
              style="background-image:url(https://i.loli.net/2020/01/31/Tp3bE5FCeBNAjSI.jpg)"
            >
              <div class="article-cc"></div>
              <div class="article">
                <div class="article-title">文章标题</div>
                <div class="article-txt">文章简介</div>
                <div class="article-qt">
                  <i class="iconfont icon-browse"></i>
                  点击量：&nbsp;
                  <i class="iconfont icon-time"></i>
                  发布时间：
                </div>
              </div>
            </div>
            <!-- </nuxt-link> -->
          </div>
          <div class="article-li">
            <!-- <nuxt-link :to="{name:'content' ,query:{id:book.id}}"> -->
            <div
              class="article-con"
              style="background-image:url(https://i.loli.net/2020/01/31/Tp3bE5FCeBNAjSI.jpg)"
            >
              <div class="article-cc"></div>
              <div class="article">
                <div class="article-title">文章标题</div>
                <div class="article-txt">文章简介</div>
                <div class="article-qt">
                  <i class="iconfont icon-browse"></i>
                  点击量：&nbsp;
                  <i class="iconfont icon-time"></i>
                  发布时间：
                </div>
              </div>
            </div>
            <!-- </nuxt-link> -->
          </div>
        </div>
      </div>

      <div class="book-left">
        <!-- 网站数据统计 -->
        <div class="aside">
          <div class="t-aside-statistics">
            <div class="t-statistics-title">
              <i class="iconfont icon-icon_index_line" aria-hidden="true"></i>文章统计
            </div>
            <ul class="t-statistics-ul">
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  最近的文章：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Html：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Css：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Javascript：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Jquery：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Vue：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Nuxt：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  WeChat：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Golang：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  MySql：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
              <li>
                <nuxt-link :to="{name:''}" class="t-statistics-a" tag="a">
                  Redis：
                  <span>(&nbsp;{{article}}&nbsp;)</span>
                </nuxt-link>
              </li>
            </ul>
          </div>
        </div>
        <!-- 技术群 -->
        <div class="group">
          <div class="group-title">
            <i class="iconfont icon-xiaoxi" aria-hidden="true"></i>
            交流探讨（QQ群）
          </div>
          <div class="group-p">xxxxxxxxx</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      article: "123"
    };
  }
};
</script>

<style lang="less" scoped>
.book {
  padding-top: 100px;
  padding-bottom: 60px;
  .book-left {
    width: 25%;
    height: auto;
    float: left;
    display: block;
    .aside,
    .friend {
      width: 100%;
      height: auto;
      background-color: #fff;
      border-radius: 8px;
    }
    .t-aside-statistics {
      padding: 20px 10px;
    }
    .t-statistics-title {
      padding: 10px;
      border-bottom: 1px solid #eee;
    }
    .t-statistics-ul {
      padding: 20px 6px;
    }
    .t-statistics-ul li {
      padding: 4px 10px;
    }
    .t-statistics-ul li .t-statistics-a span {
      float: right;
      color: #33cb98;
    }
    .icon-icon_index_line {
      color: #0080ff;
    }
    .t-statistics-a {
      color: #737088;
    }
    .t-statistics-ul li:hover {
      background-color: #33cb98;
      border-radius: 4px;
      cursor: pointer;
      transition: 0.2s all;
    }
    .t-statistics-ul li:hover > .t-statistics-a,
    .t-statistics-ul li:hover > .t-statistics-a span {
      color: #ffffff;
    }
    .group {
      margin-top: 20px;
      width: 100%;
      height: auto;
      background-color: #fff;
      border-radius: 8px;
      padding: 20px 10px;
    }

    .group-title {
      padding: 10px;
      border-bottom: 1px solid #eee;
    }

    .group-p {
      padding: 10px;
    }
  }
  .book-right {
    width: 75%;
    height: auto;
    float: left;
    display: block;
    padding-right: 20px;
    .article-ul {
      background-color: #ffffff;
      border-radius: 8px;
      .article-li {
        padding: 20px;
        border-radius: 0px;
      }
    }
  }
}
</style>