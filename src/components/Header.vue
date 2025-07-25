<template>
  <div class="header">
    <div class="nav-bar">
      <div class="hamburger" @click="toggleMenu" :class="{ 'is-active': isMenuOpen }">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div class="nav-links" :class="{ 'is-open': isMenuOpen }">
        <router-link to="/" @click="closeMenu">About me</router-link>
        <router-link to="/other-projects" @click="closeMenu">Projects</router-link>
        <router-link to="/game-projects" @click="closeMenu">Games</router-link>
        <router-link to="/resume" @click="closeMenu">Resume</router-link>
        <router-link to="/contact" @click="closeMenu">Contact</router-link>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Header",
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    closeMenu() {
      this.isMenuOpen = false;
    }
  }
});
</script>

<style scoped lang="less">
@import '../css/variables.less';

.header {
  width: 100%;
  background-color: #FFFFFF;
  position: relative;
  z-index: 1000;
}

.nav-bar {
  text-align: right;
  padding: 20px;
  line-height: 3em;
}

.nav-links {
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

.hamburger {
  display: none;
  flex-direction: column;
  justify-content: space-between;
  width: 30px;
  height: 21px;
  cursor: pointer;
  position: absolute;
  right: 20px;
  top: 20px;
  z-index: 100;

  span {
    display: block;
    height: 3px;
    width: 100%;
    background-color: #A67F5D;
    transition: all 0.3s ease;
  }

  &.is-active {
    span {
      &:first-child {
        transform: translateY(9px) rotate(45deg);
      }
      &:nth-child(2) {
        opacity: 0;
      }
      &:last-child {
        transform: translateY(-9px) rotate(-45deg);
      }
    }
  }
}

a {
  text-transform: uppercase;
  margin-left: 15px;
  margin-right: 15px;
  padding-bottom: 8px;
  white-space: nowrap;
  display: inline-block;
  color: #A67F5D !important;
  opacity: 0.8 !important;
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
  border-bottom: 2px solid #A67F5D !important;
}

@media only screen and (max-width: 620px) {
  .hamburger {
    display: flex;
  }

  .nav-links {
    display: none;
    flex-direction: column;
    position: absolute;
    top: 0;
    right: 0;
    background-color: #FFFFFF;
    width: 200px;
    padding: 60px 20px 20px;
    box-shadow: -2px 2px 10px rgba(0, 0, 0, 0.1);
    transform: translateX(100%);
    transition: transform 0.3s ease;

    &.is-open {
      display: flex;
      transform: translateX(0);
    }

    a {
      margin: 10px 0;
      font-size: 1.1em;
      width: 100%;
      text-align: left;
      padding: 10px 0;
    }
  }
}
</style>
