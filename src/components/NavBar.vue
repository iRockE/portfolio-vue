<template>
  <nav>
    <router-link to="/" class="brand-logo"><img src="@/assets/logo.png" alt="" ></router-link>
    <div class="nav-tabs">
      <router-link to="/experience">Experience</router-link>
      <router-link to="/projects">Projects</router-link>
      <router-link to="/resume">Resume</router-link>
    </div>
    <button type="button" class="hamburger-menu" @click="showNavMobile"></button>
  </nav>
  <NavMobile ref="navMobile" />
</template>

<script>
import NavMobile from "@/components/NavMobile";

export default {
  name: "NavBar",
  components: {
    NavMobile
  },
  methods: {
    showNavMobile() {
      this.$refs.navMobile.show = true;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
nav {
  color: #fff;
  background-color: #546e7a;
  width: 100%;
  height: 56px;
  line-height: 56px;
  box-shadow: 0 2px 2px 0 rgb(0 0 0 / 14%), 0 3px 1px -2px rgb(0 0 0 / 12%), 0 1px 5px 0 rgb(0 0 0 / 20%);
  @include sm {
    height: 64px;
    line-height: 64px;
  }
  .nav-tabs {
    float: right;
    a {
      text-decoration: none;
      transition: background-color .3s;
      float: left;
      font-size: 1rem;
      color: #fff;
      display: none;
      padding: 0 15px;
      cursor: pointer;
      &:hover {
        background-color: rgba(0,0,0,0.1);
      }
      @include lg {
        display: block;
      }
    }
  }
  .brand-logo {
    position: absolute;
    padding: 0;
    height: 56px;
    left: 50%;
    transform: translateX(-50%);
    @include sm {
      height: 64px;
    }
    @include lg {
      left: auto;
      transform: none;
    }
    img {
      padding: 0 20px;
      width: 56px;
      @include sm {
        width: 64px;
      }
    }
  }
  .hamburger-menu {
    background-color: transparent;
    color: inherit;
    border: none;
    padding: 0;
    cursor: pointer;
    outline: inherit;
    float: left;
    top: 0;
    background-image: url(../assets/menu.svg);
    background-repeat: no-repeat;
    background-position: center;
    height: 100%;;
    width: 64px;
    @include lg {
      display: none;
    }
  }
}
</style>
