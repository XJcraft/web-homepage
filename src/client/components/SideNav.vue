<template>
  <nav class="side-nav">
    <div class="container">
      <nuxt-link to="/" class="logo">
        <img src="/logo.png" alt="XJCraft" />
      </nuxt-link>
      <div class="operate">
        <el-popover width="300" trigger="hover">
          <a slot="reference" class="link">微信公众号</a>
          <img class="qrcode" src="/qrcode.jpg" alt="二维码" />
        </el-popover>
        <a class="link" href="https://space.bilibili.com/8980695">Bilibili</a>
        <!-- <a class="link" href="">wiki</a> -->
        <a class="link" href="http://map.locsian.com/">卫星地图</a>
        <!-- <a class="link" href="">论坛</a> -->
        <div class="underline"></div>
        <a class="link" href="https://apply.xj.locsian.com/req">注册</a>
        <!-- <a class="link" href="">登录</a> -->
      </div>
    </div>
  </nav>
</template>
<script>
export default {}
</script>
<style lang="less">
.side-nav {
  height: 100px;

  .container {
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    margin: 0 auto;
  }

  .logo {
    height: 54px;
    display: inline-block;

    img {
      height: 100%;
      width: 100%;
    }
  }

  .operate {
    display: flex;
    flex-wrap: wrap;
    .link {
      position: relative;
      display: inline-block;
      text-decoration: none;
      font-weight: 400;
      color: rgba(255, 255, 255, 1);
      line-height: 24px;
      padding: 0 20px;
      text-shadow: 0 1px 1px rgba(0, 0, 0, 0.3);
      white-space: nowrap;
      transition: all 0.5s;

      &::before {
        content: '';
        position: absolute;
        bottom: -8px;
        left: calc(50% - 15px);
        height: 2px;
        width: 30px;
        background: #fc9a1b;
        transition: all 0.3s;
        transform: scale(0);
      }
      &:hover::before {
        transform: scale(1);
      }

      &:hover {
        color: #fc9a1b;
      }
    }
    .underline::before {
      display: inline-block;
      content: '';
      background: rgba(255, 255, 255, 1);
      width: 1px;
      height: 20px;
      margin: 0 20px;
    }
  }
}
.qrcode {
  width: 100%;
  height: 100%;
}
</style>
