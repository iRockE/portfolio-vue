<template>
  <transition name="fade">
    <div v-if="show" class="nav-mobile-overlay" @click="show = false"></div>
  </transition>
  <transition name="slide">
    <nav v-if="show">
      <router-link to="/experience" @click="show = false">Experience</router-link>
      <router-link to="/projects" @click="show = false">Projects</router-link>
      <router-link to="/resume" @click="show = false">Resume</router-link>
    </nav>
  </transition>
</template>

<script>
export default {
  name: "NavMobile",
  data() {
    return {
      show: false
    }
  },
  watch: {
    show(newShow) {
      document.body.style.overflow = newShow ? "hidden" : null;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.nav-mobile-overly {
  z-index: 100;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 120vh;
  background-color: rgba(0,0,0,0.5);
}
nav {
  z-index: 101;
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

/*#region Transitions*/
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease;
}
.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
.slide-enter-active,
.slide-leave-active {
  transition: transform 0.3s ease;
}
.slide-enter-from,
.slide-leave-to {
  transform: translateX(-105%);
}
/*#endregion*/
</style>
