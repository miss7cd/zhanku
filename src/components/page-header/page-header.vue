<template>
  <header class="page-header">
    <div class="logo">
      <img src="@/assets/images/logo.svg" alt>
    </div>
    <ul class="menu-list-wrapper">
      <li class="item">
        <div class="menu-list-box">首页</div>
      </li>
      <li>
        <div class="menu-list-box">发现</div>
        <div class="drop-down">
          <div class="drop-down-item"></div>
        </div>
      </li>
      <li>
        <div class="menu-list-box">同城</div>
      </li>
      <li>
        <div class="menu-list-box">职位</div>
      </li>
      <li>
        <div class="menu-list-box">活动</div>
      </li>
      <li>
        <div class="menu-list-box">正版素材</div>
      </li>
      <li>
        <div class="menu-list-box">课程</div>
      </li>
    </ul>
    <div class="login-wrapper">
      <div class="login">登陆</div>
      <span></span>
      <div class="register">注册</div>
    </div>
  </header>
</template>

<script>
export default {}
</script>

<style lang="less">
@import "./../../assets/less/mixin.less";
.page-header {
  padding-left: 30px;
  padding-right: 30px;
  width: 100%;
  background-color: @theme_color;
  display: flex;
  align-items: center;
  justify-content: space-between;
  .logo {
    img {
      width: 120px;
      height: 20px;
    }
  }
  .menu-list-wrapper {
    display: flex;
    // flex: 1;
    li {
      .menu-list-box {
        font-size: 14px;
        line-height: 20px;
        color: #333;
        padding: 10px 20px;
        cursor: pointer;
        &:hover {
          background-color: #333;
          color: #fff;
        }
      }
      &.active .menu-list-box {
        font-weight: bold;
      }
    }
  }
  .login-wrapper{
      display: flex;
      align-items: center;
      .login,.register{
          padding: 10px;
      }
      span{
          display: block;
          width: 1px;
          height: 14px;
          background-color: #333;
      }
  }
}
</style>
