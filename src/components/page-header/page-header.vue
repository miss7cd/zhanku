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
  </header>
</template>

<script>
export default {}
</script>

<style lang="less">
@import "./../../assets/less/mixin.less";
.page-header {
  width: 100%;
  background-color: @theme_color;
  display: flex;
  align-items: center;
  .logo {
    img {
      width: 120px;
      height: 20px;
    }
  }
  .menu-list-wrapper {
    display: flex;
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
}
</style>
