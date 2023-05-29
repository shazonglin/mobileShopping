<template>
  <div class="docker">
    <div class="docker_item docker_item--active">
      <div class="iconfont">&#xe617;</div>
      <div class="docker_title">首页</div>
    </div>
    <div class="docker_item">
      <div class="iconfont">&#xe6af;</div>
      <div class="docker_title">购物车</div>
    </div>
    <div class="docker_item">
      <div class="iconfont">&#xe608;</div>
      <div class="docker_title">订单</div>
    </div>
    <div class="docker_item">
      <div class="iconfont">&#xe78b;</div>
      <div class="docker_title">我的</div>
    </div>
  </div>
</template>

<style lang="scss">
.docker {
  position: absolute;
  display: flex;
  padding: 0 0.18rem;
  box-sizing: border-box;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 0.49rem;
  border-top: 1px solid #f1f1f1;
  &_item {
    flex: 1;
    text-align: center;
    .iconfont {
      margin: 0.07rem 0 0.02rem 0;
      font-size: 0.18rem;
    }
    &--active {
      color: #1fa4fc;
    }
  }
  &_title {
    font-size: 20px;
    transform: scale(0.5, 0.5);
    transform-origin: center top;
  }
}
</style>
