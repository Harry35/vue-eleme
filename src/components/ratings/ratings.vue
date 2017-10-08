<template>
  <div class="ratings">
    <div class="ratings-content">
      <div class="overview">
        <div class="overview-left">
          <h1 class="score">{{seller.score}}</h1>
          <div class="title">综合评分</div>
          <div class="rank">高于周边商家{{seller.rankRate}}%</div>
        </div>
        <div class="overview-right"></div>
      </div>
    </div>
  </div>
</template>

<script type="text/exmascript-6">
  export default {
    props: {
      seller: {
        type: Object
      }
    }
  };
</script>

<style lang="stylus" rel="stylesheet/stylus">
.ratings
  postition: absolute
  top: 174px
  bottom: 0
  left: 0
  width: 100%
  overflow: hidden
  .overview
    display: flex
    padding: 18px
    .overview-left
      flex: 0 0 137px
      width: 137px
    .overview-right
      flex: 1
      padding-left: 24px
</style>
