<!--  -->
<template>
  <div :class="$style.header">
    <span :class="$style.left">
      <em>注册</em>
      &nbsp;|&nbsp;
      <em>下载</em>
    </span>
    <btn :class="$style.btnDownload">App下载</btn>
  </div>
</template>

<script>
import btn from '../code/btn.vue';
export default {
  components: {
    btn
  },
  data () {
    return {
    };
  }
}

</script>
<style lang='scss' module>
.header{
  height:100xp;
  line-height: 100px;
  color: #666;
  position: fixed;
  left: 0;
  top: 0;
  right: 0;
  background: #fff url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
  background-size: auto 50%;
  z-index: 100;
  font-size: 32px;
  .left{
    font-size: 28px;
    height: 30px;
    line-height: 30px;
    margin: 17px 0 0 18px
  }
  .btnDownload{
    float: right;
    font-size: 24px;
    border-width: 0;
    height: 56px;
    line-height: 56px;
    min-width: 120px;
    padding: 0;
    border-radius: 4px;
    margin: 28px 24px 0 0;
  }
}
</style>