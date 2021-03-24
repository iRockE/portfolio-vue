<template>
  <div class = "back-to-top-wrapper">
    <a @click="scrollToTop">Back to Top</a>
  </div>
</template>

<script>
export default {
  name: "BackToTop",
  methods: {
    scrollToTop() {
      window.scrollTo({
          top: 0, 
          left: 0, 
          behavior: 'smooth' 
      });
    }
  }
};
</script>

<style lang="scss" scoped>
.back-to-top-wrapper {
  height: 4rem;
  width: 100%;    
  text-align: right;
  padding: 30px 0 0;
  a {
    color: $font-grey-3;
    text-decoration: none;
    font-size: 1.2rem;
    line-height: 4rem;
    white-space: nowrap;
    transition: opacity .2s;
    cursor: pointer;
    &:hover {
      opacity: 0.9;
    }
  }
}
</style>
