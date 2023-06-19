<template>
  <!-- top area -->
  <div class="wrapper">
    <div class="location">
      <span class="iconfont iconfont_position">&#xe7f3;</span>
      xxxxxxxxxxxxxxxxxxxxx
      <span class="iconfont iconfont_notice">&#xe60d;</span>
    </div>
    <!-- search&banner area -->
    <div class="search">
      <span class="iconfont">&#xe600;</span>
      <span class="search_text">xxxxxxxxxxxxxxxxxxxxx</span>
    </div>
    <div class="banner">
      <img class="banner_img" src="./assets/banner.png" alt="" />
      <!-- <img class="banner_img" src="./assets/file.jpeg" alt="" /> -->
    </div>
  </div>

  <!-- bottom area -->
  <div class="docker">
    <div class="docker_item docker_item--active">
      <div class="iconfont">&#xe617;</div>
      <div class="docker_title">HOME</div>
    </div>
    <div class="docker_item">
      <div class="iconfont">&#xe6af;</div>
      <div class="docker_title">CART</div>
    </div>
    <div class="docker_item">
      <div class="iconfont">&#xe608;</div>
      <div class="docker_title">ORDER</div>
    </div>
    <div class="docker_item">
      <div class="iconfont">&#xe78b;</div>
      <div class="docker_title">MY</div>
    </div>
  </div>
</template>

<style lang="scss">
@import "./style/variable.scss";
@import "./style/mixins.scss";

// Top area
.wrapper {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 5rem;
  padding: 0 1.8rem;
}
.location {
  color: $content-fontColor;
  position: relative;
  padding: 1.6rem 2.4rem 1.6rem 0;
  line-height: 2.2rem;
  font-size: 1.6rem;
  @include ellipse;
  .iconfont_position {
    position: relative;
    margin-right: 1.6rem;
    top: 0.2rem;
    font-size: 2rem;
  }
  .iconfont_notice {
    position: absolute;
    font-size: 2rem;
    right: 0;
    top: 1.8rem;
  }
}

// Search&Banner area
.search {
  vertical-align: middle;
  background-color: #f5f5f5;
  color: #b7b7b7;
  line-height: 3.2rem;
  border-radius: 1.6rem;
  margin-bottom: 1.2rem;
  .iconfont {
    display: inline-block;
    position: relative;
    top: 0.2rem;
    padding: 0 0.8rem 0 1.6rem;
    font-size: 2rem;
  }
  &_text {
    display: inline-block;
    font-size: 1.6rem;
  }
}

.banner {
  &_img {
    width: 100%;
  }
}

// Bottom area
.docker {
  position: absolute;
  display: flex;
  padding: 0 1.8rem;
  box-sizing: border-box;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  height: 4.9rem;
  border-top: 0.1rem solid #f1f1f1;
  color: $content-fontColor;
  &_item {
    flex: 1;
    text-align: center;
    .iconfont {
      margin: 0.7rem 0 0.2rem 0;
      font-size: 1.8rem;
    }
    &--active {
      color: #1fa4fc;
    }
  }
  &_title {
    font-size: 2rem;
    transform: scale(0.5, 0.5);
    transform-origin: center top;
  }
}
</style>
