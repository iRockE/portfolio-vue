<template>
  <a target="_blank" :href="link">
    <slot></slot>
  </a>
</template>

<script>
export default {
  name: "LinkButton",
  props: ["link"]
};
</script>

<style lang="scss" scoped>
a {
  display: inline-block;
  text-decoration: none;
  color: #fff;
  background-color: $button-color;
  text-align: center;
  letter-spacing: .5px;
  transition: .3s;
  vertical-align: middle;
  -webkit-tap-highlight-color: transparent;
  user-select: none;
  font-size: 14px;
  border: none;
  border-radius: 2px;
  cursor: pointer;
  height: 36px;
  line-height: 36px;
  padding: 0 16px;
  text-transform: uppercase;
  box-shadow: 0 2px 2px 0 rgb(0 0 0 / 14%), 0 3px 1px -2px rgb(0 0 0 / 12%), 0 1px 5px 0 rgb(0 0 0 / 20%);
  &:hover {
    background-color: $button-hover-color;
    box-shadow: 0 3px 3px 0 rgb(0 0 0 / 14%), 0 1px 7px 0 rgb(0 0 0 / 12%), 0 3px 1px -1px rgb(0 0 0 / 20%);
  }
}
</style>
