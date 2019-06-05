<template>
  <div class="header">
    <div class="header_l">
      <span class="iconfont back_btn">&#xe624;</span>
    </div>
    <div class="header_m">
      <span class="iconfont">&#xe632;</span>
      城市旅游景点
    </div>
    <div class="header_r">
      城市
      <span class="iconfont sel">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
@import '~@/assets/styles/common.styl';

.header {
  display: flex;
  height: 0.86rem;
  line-height: 0.86rem;
  background: $bg;
  color: #ffffff;

  .header_l {
    width: 0.64rem;
    float: left;

    .back_btn {
      text-align: left;
      font-size: 0.4rem;
    }
  }

  .header_r {
    width: 1.24rem;
    float: left;
    text-align: center;

    .sel {
      font-size: 0.24rem;
      margin-left: -0.04rem;
    }
  }

  .header_m {
    flex: 1;
    background: #ffffff;
    border-radius: 0.1rem;
    height: 0.64rem;
    margin-top: 0.12rem;
    padding-left: 0.2rem;
    color: #cccccc;
    line-height: 0.64rem;
  }
}
</style>
