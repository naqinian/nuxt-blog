<template>
  <div class="index content-top">
    <!--  -->
    <div class="index-banner">
      <div class="t-container">
        <div class="banner-text">
          <!-- <img class="banner-img" src="~/assets/img/2020462134088922.jpg" /> -->
          <div class="banner-div">
            <p class="banner-name">从前有个如初。</p>
            <p class="banner-professional">一名前端开发爱好者，从事网页设计和开发。</p>
            <p class="banner-professional">喜欢简约和一切美好的事物！</p>
            <p class="banner-professional">喜欢美食、音乐、电影、游戏、编程...</p>
          </div>
          <a href="#" class="banner-btn">About&nbsp;me</a>
        </div>
      </div>
    </div>
    <!--  -->
    <div class="index-article">
      <div class="t-container">
        <div class="index-title">
          <span>文章推荐</span>
        </div>
        <div class="article-ul">
          <div class="article-li">
            <!-- <nuxt-link :to="{name:'content' ,query:{id:book.id}}"> -->
              <div
                class="article-con"
                style="background-image:url(https://i.loli.net/2020/01/31/Tp3bE5FCeBNAjSI.jpg)"
              >
                <div class="article-cc"></div>
                <div class="article">
                  <div class="article-title">文章标题</div>
                  <div class="article-txt">文章摘要</div>
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
                  <div class="article-txt">文章摘要</div>
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
                  <div class="article-txt">文章摘要</div>
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
        <div class="index-btn">
          <nuxt-link :to="{name:'book'}" tag="a">book&nbsp;me</nuxt-link>
        </div>
      </div>
    </div>
    <!--  -->
    <div class="index-resources">
      <div class="t-container">
        <div class="index-title">
          <span>图片推荐</span>
        </div>
        <div class="resources">
          <div class="gallery">
            <a href="~/assets/img/i8.jpg" class="image">
              <img src="~/assets/img/i8.jpg" alt />
            </a>
            <a href="~/assets/img/i7.jpg" class="image">
              <img src="~/assets/img/i7.jpg" alt />
            </a>
            <a href="~/assets/img/i6.jpg" class="image">
              <img src="~/assets/img/i6.jpg" alt />
            </a>
            <a href="~/assets/img/i5.jpg" class="image">
              <img src="~/assets/img/i5.jpg" alt />
            </a>
            <a href="~/assets/img/i4.jpg" class="image">
              <img src="~/assets/img/i4.jpg" alt />
            </a>
            <a href="~/assets/img/i3.jpg" class="image">
              <img src="~/assets/img/i3.jpg" alt />
            </a>
            <a href="~/assets/img/i2.jpg" class="image">
              <img src="~/assets/img/i2.jpg" alt />
            </a>
            <a href="~/assets/img/i1.jpg" class="image">
              <img src="~/assets/img/i1.jpg" alt />
            </a>
          </div>
        </div>
        <div class="index-btn">
          <nuxt-link :to="{name:'resources'}" tag="a">resources&nbsp;me</nuxt-link>
        </div>
      </div>
    </div>
    <!--  -->
    <div class="index-link">
      <div class="t-container">
        <div class="index-title">
          <span>友&nbsp;人&nbsp;帐</span>
        </div>
        <div class="link">
          <div class="user">
            <div class="container">
              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m1.jpg" />
                    <h3>Design</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>
              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m2.jpg" />
                    <h3>Code</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>

              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m3.jpg" />
                    <h3>Launch</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>

              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m4.jpg" />
                    <h3>Launch</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>

              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m1.jpg" />
                    <h3>Design</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>
              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m2.jpg" />
                    <h3>Code</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>

              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m3.jpg" />
                    <h3>Launch</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>
              <div class="card">
                <div class="face face1">
                  <div class="content">
                    <img src="~/assets/img/m3.jpg" />
                    <h3>Launch</h3>
                  </div>
                </div>
                <div class="face face2">
                  <div class="content">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cum cumque minus iste veritatis provident at.</p>
                    <a href="#">Read More</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="index-btn">
          <a href="#" class>link&nbsp;me</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.index-banner {
  width: 100%;
  min-height: 930px;
  background-image: -webkit-linear-gradient(
      top,
      rgba(0, 0, 0, 0.1),
      rgba(0, 0, 0, 0.1)
    ),
    url("../assets/img/1.jpg");
  background-attachment: fixed;
  background-position: center center;
  background-repeat: no-repeat;
  position: relative;
  -webkit-background-size: 100%;
  -moz-background-size: 100%;
  -ms-background-size: 100%;
  background-size: 100%;
  .banner-text {
    padding-top: 260px;
    padding-left: 30px;
    color: #000;
    .banner-img {
      width: 180px;
      height: auto;
      border: 4px solid #d7d8d6;
      box-shadow: 10px 10px 20px 0px #c3c4c2;
    }
    .banner-div {
      padding: 40px 0 20px 0;
      .banner-name {
        font-size: 50px;
        padding: 0 0 10px 0;
        font-weight: 700;
      }
      .banner-professional {
        font-size: 20px;
        padding: 2px 0;
      }
    }
    .banner-btn {
      background-color: #33cb98;
      color: #fff;
      width: 180px;
      border: 2px solid #33cb98;
      border-radius: 999px;
      font-size: 16px;
      letter-spacing: 0.1em;
      display: inline-block;
      text-align: center;
      padding: 10px 0;
    }
    .banner-btn:hover {
      opacity: 0.6;
      background-color: #fff;
      color: #000;
      border: 2px solid #fff;
      transition: 0.6s all;
    }
  }
}

.index-article,
.index-resources,
.index-link {
  padding-bottom: 60px;
}

.index-resources {
  background-color: #fff;
}



// 文章分类
.article-ul {
  width: 100%;
  height: auto;
  padding-top: 60px;
}

// 资源分享
.index-resources {
  background-color: #f9faf9;
}

.resources {
  padding-top: 60px;
  
}



.index-btn {
  width: 100%;
  height: auto;
  padding: 60px 0 0 0;
  text-align: center;
  a {
    background-color: #33cb98;
    color: #fff;
    width: 180px;
    border: 2px solid #33cb98;
    border-radius: 999px;
    font-size: 16px;
    letter-spacing: 0.1em;
    display: inline-block;
    text-align: center;
    padding: 10px 0;
  }
  a:hover{
    opacity: 0.6;
      background-color: #fff;
      color: #000;
      border: 2px solid #33cb98;
      transition: 0.6s all;
  }
}
</style>
