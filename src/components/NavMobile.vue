<template>
  <div class="nav-mobile" @click="$emit('exit')">
    <nav>
      <router-link to="/experience">Experience</router-link>
      <router-link to="/projects">Projects</router-link>
      <router-link to="/resume">Resume</router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: "NavMobile",
  props: {
    show: {
      type: Boolean,
      default: false,
      required: true
    }
  },
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
  z-index: 100;
}
</style>
