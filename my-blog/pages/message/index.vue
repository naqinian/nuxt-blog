<template>
  <div class="message">
    <div class="t-container">
      <div class="message-left">
        <div class="message-wang">
          <!-- 富文本 -->
          <div class="wang-txt">
            <div id="div2"></div>
            <div id="div1"></div>
            <div class="wang">
              <button @click="getContent()">提交信息</button>
            </div>
          </div>
          <!-- 列表 -->
          <ul class="message-ul">
            <li class="message-li">
              <div class="message-li-left">
                <img src="~/assets/img/m1.jpg" />
                <div class="message-li-name">如初</div>
              </div>
              <div class="message-li-right">
                <div class="message-li-right-related">
                  <i class="iconfont icon-time"></i>
                  2020-05-10
                </div>
                <div class="message-li-right-content">内容</div>
                <div class="message-li-right-botton">回复</div>
              </div>
              <div class="message-reply">
                <div class="message-li-left">
                  <img src="~/assets/img/m1.jpg" />
                  <div class="message-li-name">如初</div>
                </div>
                <div class="message-li-right">
                  <div class="message-li-right-related">
                    回复&nbsp;&nbsp;
                    <span class="message-hf">如初。</span>
                    <i class="iconfont icon-time"></i>
                    2020-05-10
                  </div>
                  <div class="message-li-right-content">内容</div>
                  <div class="message-li-right-botton">回复</div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
      <div class="message-right">
        <!-- 留言统计 -->
        <div class="aside">
          <div class="t-aside-statistics">
            <div class="t-statistics-title">
              <i class="iconfont icon-icon_index_line" aria-hidden="true"></i>留言统计
            </div>
            <ul class="t-statistics-ul">
              <li>
                上次查看时间：
                <span>(&nbsp;{{article}}&nbsp;)</span>
              </li>
              <li>
                留言总数：
                <span>(&nbsp;{{article}}&nbsp;)</span>
              </li>
              <li>
                QQ用户访问总数：
                <span>(&nbsp;{{article}}&nbsp;)</span>
              </li>
            </ul>
          </div>
        </div>
        <!-- 最近访客 -->
        <div class="friend">
          <div class="friend-title">
            <div class="t-statistics-title">
              <i class="iconfont icon-icon_patriarch" aria-hidden="true"></i>最近访客
            </div>
            <div class="friend-ul">
              <div class="friend-li">
                <p>
                  <img src="~/assets/img/m2.jpg" />
                </p>
                <div class="friend-name">
                  <span title="aink.name">aink.name</span>
                </div>
              </div>
              <div class="friend-li">
                <p>
                  <img src="~/assets/img/m3.jpg" />
                </p>
                <div class="friend-name">
                  <span title="aink.name">aink.name</span>
                </div>
              </div>
              <div class="friend-li">
                <p>
                  <img src="~/assets/img/m4.jpg" />
                </p>
                <div class="friend-name">
                  <span title="aink.name">aink.name</span>
                </div>
              </div>
              <div class="friend-li">
                <p>
                  <img src="~/assets/img/m4.jpg" />
                </p>
                <div class="friend-name">
                  <span title="aink.name">aink.name</span>
                </div>
              </div>
              <div class="friend-li">
                <p>
                  <img src="~/assets/img/m4.jpg" />
                </p>
                <div class="friend-name">
                  <span title="aink.name">aink.name</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const E = process.browser ? require("wangeditor") : undefined;
export default {
  data() {
    return {
      article: "4399"
    };
  },
  mounted() {
    var editor = new E("#div1", "#div2");
    // 自定义菜单配置
    editor.customConfig.menus = ["emoticon"];
    editor.customConfig.zIndex = 100;
    editor.customConfig.onchange = html => {
      this.editorContent = html;
    };
    editor.create();
  },
  methods: {
    getContent: function() {
      this.tips = "😜，我还没写接口！";
      this.isLink = true;
      setTimeout(() => {
        this.isLink = false;
        this.tips = "";
      }, 3000);
    }
  }
};
</script>

<style lang="less" scoped>
.message {
  padding-top: 100px;
  padding-bottom: 60px;
  .message-left {
    width: 75%;
    height: auto;
    float: left;
    display: block;
    padding-right: 20px;
    .message-wang {
      background-color: #fff;
      padding: 20px 30px;
      /* 富文本 */
      #div2 {
        width: 100%;
        height: 100px;
        border: 1px solid #e1e8ed;
      }
      .wang-txt .wang {
        padding: 0px 0px 20px 0px;
        text-align: right;
        margin-top: -20px;
        button {
          color: #fff;
          background-color: #33cb98;
          border: 1px solid #33cb98;
          padding: 9px 10px;
          border-radius: 4px;
        }
        button:hover {
          opacity: 0.8;
          cursor: pointer;
          transition: 0.4s all;
        }
      }
    }
    /* 留言列表 */
    .message-ul {
      width: 100%;
      height: auto;
      margin: 20px 0;
    }
    .message-li {
      width: 100%;
      height: auto;
      padding: 10px 0 16px 0;
      border-bottom: 1px solid #eee;
      position: relative;
    }
    .message-li:last-child {
      border-bottom: none;
    }
    .message-li-left {
      width: 120px;
      height: auto;
      text-align: center;
      padding: 10px;
      position: absolute;
    }
    .message-li-left img {
      width: 60px;
      height: 60px;
      padding: 4px;
      border-radius: 50%;
    }
    .message-li-name {
      color: #869da7;
    }
    .message-li-right {
      width: 100%;
      padding: 0px 6px 0px 130px;
      text-align: justify;
      text-justify: newspaper;
      word-break: break-all;
    }
    .message-li-right-content {
      width: 100%;
      min-height: 60px;
    }
    .message-li-right-related span {
      padding-right: 10px;
    }
    .message-li-right-botton {
      text-align: right;
    }
  }

  .message-right {
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
    .t-statistics-ul li span {
      float: right;
      color: #33cb98;
    }
    .icon-icon_index_line {
      color: #0080ff;
    }
    .friend {
      margin-top: 20px;
      width: 100%;
      height: auto;
      background-color: #fff;
      border-radius: 8px;
    }
    .friend-title {
      padding: 20px 10px;
    }

    .friend-title .fa {
      margin-right: 10px;
      width: 20px;
      height: 20px;
    }
    .t-statistics-title {
      padding: 10px;
      border-bottom: 1px solid #eee;
    }
    .friend-ul {
      margin-top: 10px;
      text-align: center;
    }

    .friend-li {
      width: 33%;
      height: 105px;
      float: left;
      padding: 10px;
    }

    .friend-li p {
      margin: 0;
      padding: 0;
    }

    .friend-li p img {
      border-radius: 10px;
    }

    .friend-li .friend-name {
      width: 80%;
      height: auto;
      text-overflow: ellipsis;
      overflow: hidden;
      word-break: break-all;
      white-space: nowrap;
      margin: 0 auto;
    }

    .friend-li .friend-name span {
      color: #505051;
    }

    .friend-ul::after {
      content: "";
      display: table;
      clear: both;
    }
  }
}

.message-reply:nth-child {
  border: none;
}
.message-ul .message-li .message-reply {
  min-height: 100px;
  padding: 15px;
  background: #f7f7f9;
  border-radius: 4px;
  margin-top: 20px;
  margin-left: 68px;
  margin-bottom: 4px;
}

.message-hf {
  color: #0096ff;
}
</style>