<template>
  <div class = "breadcrumb-wrapper">
    <nav>
      <router-link v-for="(item, index) in trail" :key="item" :to="`/${(index == 0) ? '' : item.toLowerCase()}`">
        <span v-if="index != 0"> > </span>{{item}}
      </router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: "NavBreadcrumb",
  props: {
    trail: Array
  }
};
</script>

<style lang="scss" scoped>
.breadcrumb-wrapper {
  height: 4rem;
  width: 100%;
  nav {
    a {
      color: $font-grey-3;
      text-decoration: none;
      font-size: 1.2rem;
      line-height: 4rem;
      white-space: nowrap;
      transition: opacity .2s;
      &:hover {
        opacity: 0.9;
      }
    }
  }
}
</style>
