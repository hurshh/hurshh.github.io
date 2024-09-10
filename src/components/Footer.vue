<template>
  <div class="footer">
    
    <div class="left"> <strong>Made with ❤️ by Harsh</strong></div>
    <div class="right" > <strong>Reach me at <a href="mailto:hurshrao@gmail.com">hurshrao@gmail.com</a> or <router-link to="/contact">through here</router-link></strong></div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Footer"
});
</script>

<style scoped lang="less">

@import '../css/variables.less';

.footer {
  background-color: @bodyBgColor;
  color: #ffffff;
  width: 100%;
  font-size: 0.8em;
  opacity: 0.7;
  padding-bottom: 30px;
}

.footer a{
  color: #FFFCFF;
}

.left, .right {
    padding-top: 10px;
    text-align: center;
  }

@media only screen and (min-width: 620px){

  .footer {
    padding: 0;
  }

  .left, .right {
    padding: 20px;
  }

  .left {
    float: left;
  }

  .right {
    float:right;
  }
}
</style>