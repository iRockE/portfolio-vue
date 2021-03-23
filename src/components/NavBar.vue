<template>
  <nav>
    <router-link to="/" class="brand-logo"><img src="@/assets/logo.png" alt="" ></router-link>
    <div class="nav-tabs">
      <router-link to="/experience">Experience</router-link>
      <router-link to="/projects">Projects</router-link>
      <router-link to="/resume">Resume</router-link>
    </div>
    <ul class="nav-mobile">
      <li><a href="/experience">Experience</a></li>
      <li><a href="/projects">Projects</a></li>
      <li><a href="/resume">Resume</a></li>
    </ul>
    <a href="#" data-target="nav-mobile" class="sidenav-trigger">
      <i class="material-icons">menu</i>
    </a>
  </nav>
</template>

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
      @include sm {
        height: 64px;
      }
      img {
        padding: 0 20px;
        width: 56px;
        @include sm {
          width: 64px;
        }
      }
    }
}
</style>
