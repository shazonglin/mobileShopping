<template>
  <div class="docker">
    <div class="docker-item">首页</div>
    <div class="docker-item">购物车</div>
    <div class="docker-item">订单</div>
    <div class="docker-item">我的</div>
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
  background-color: rgb(203, 236, 203);
}

.docker-item {
  flex: 1;
  text-align: center;
}
</style>
