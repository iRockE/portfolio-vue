<template>
  <div class="nav-mobile" @click="$emit('exit')"></div>
  <nav>
    <router-link to="/experience" @click="$emit('exit')">Experience</router-link>
    <router-link to="/projects" @click="$emit('exit')">Projects</router-link>
    <router-link to="/resume" @click="$emit('exit')">Resume</router-link>
  </nav>
</template>

<script>
export default {
  name: "NavMobile",
  emits: ['exit']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.nav-mobile {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 120vh;
  background-color: rgba(0,0,0,0.5);
}
nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 300px;
  height: 120vh;
  background-color: #fff;

  a {
    text-decoration: none;
    color: inherit;
    display: block;
    font-size: 14px;
    font-weight: 500;
    height: 48px;
    line-height: 48px;
    padding: 0 32px;
    transition: background-color .3s;
    &:hover {
      background-color: rgba(0,0,0,0.1);
    }
  }
}
</style>
