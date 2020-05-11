<template>
  <div class="header">
    <header class="t-header">
      <div class="t-container t-header-container">
        <nuxt-link :to="{name:'index'}" class="t-header-logo">
          <img
            src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1589099276734&di=0e9d5c71d0844866b4f9c2e6e6df8b25&imgtype=0&src=http%3A%2F%2F5b0988e595225.cdn.sohucs.com%2Fq_70%2Cc_zoom%2Cw_640%2Fimages%2F20180621%2F55a7c22bc6ae4debb81c34367837460d.jpeg"
          />
        </nuxt-link>
        <ul class="t-menu" for="chk">
          <li>
            <nuxt-link :to="{name:'index'}" class="t-menu-a" tag="a">首页</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="{name:'book'}" class="t-menu-a" tag="a">笔记本</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="{name:'resources'}" class="t-menu-a" tag="a">分享</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="{name:'message'}" class="t-menu-a" tag="a">留言板</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="{name:'link'}" class="t-menu-a" tag="a">友人帐</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="{name:'about'}" class="t-menu-a" tag="a">关于我</nuxt-link>
          </li>
          <li>
            <nuxt-link :to="{name:'record'}" class="t-menu-a" tag="a">更新记录</nuxt-link>
          </li>
        </ul>
      </div>
    </header>
  </div>
</template>


<style lang="less" scoped>
.nuxt-link-exact-active {
  // color: #f7c65b;
  color: #33cb98;
}

.header {
  position: fixed;
  top: 0px;
  width: 100%;
  z-index: 1024;
  box-shadow: 0px 1px 10px rgba(189, 197, 209, 0.4);
  .t-header {
    width: 100%;
    height: 60px;
    background: #fff;
    overflow: hidden;
    .t-header-container {
      display: -ms-flexbox;
      display: flex;
      .t-header-logo {
        margin-left: 60px;
        display: block;
        img {
          width: 42px;
          height: 42px;
          margin-top: 9px;
        }
      }
      .t-menu {
        margin-left: 60px;
        li {
          float: left;
          .t-menu-a {
            padding: 22px 16px;
            line-height: 60px;
            font-weight: 600;
            font-size: 14px;
          }
          .t-menu-a:hover {
            color: #33cb98;
            cursor: pointer;
          }
        }
      }
    }
  }
}
</style>