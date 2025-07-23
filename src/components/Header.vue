<template>
  <div class="header">
    <div class="nav-bar">
      <router-link to="/">About me</router-link>
      <router-link to="/other-projects">Projects</router-link>
      <router-link to="/game-projects">Games</router-link>
<!--        <router-link to="/art">Art</router-link>-->
      <router-link to="/resume">Resume</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Header"
});
</script>

<style scoped lang="less">
@import '../css/variables.less';

.header {
  width: 100%;
  background-color: #FFFFFF;  // White background for header
}

.nav-bar {
  text-align: right;
  padding: 20px;
  line-height: 3em;
}

a {
  text-transform: uppercase;
  margin-left: 15px;
  margin-right: 15px;
  padding-bottom: 8px;
  white-space: nowrap;
  display: inline-block;
  color: #A67F5D !important;  // Warm accent color
  opacity: 0.8 !important;  // Slightly dimmed by default
  transition: all 0.3s ease;
  text-decoration: none;
  border-bottom: 2px solid transparent;
  font-weight: 500;
  letter-spacing: 0.5px;

  &:hover {
    opacity: 1 !important;
    border-bottom-color: #A67F5D;
  }
}

.router-link-exact-active {
  opacity: 1 !important;
  border-bottom: 2px solid #A67F5D !important;  // Warm accent color for active link
}

@media only screen and (max-width: 620px){
  .nav-bar {
    line-height: 2em;
  }

  a {
    margin-left: 9px;
    margin-right: 9px;
    padding-bottom: 0px;
  }
}
</style>
