<template>
    <NavBar />
    <router-view class="page-content" />
</template>

<script>
import NavBar from "@/components/NavBar";

export default {
  name: "App",
  components: {
    NavBar
  }
};
</script>

<style lang="scss">
html {
  color: rgba(0,0,0,0.87);
  font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif;
  font-weight: normal;
  font-size: 14px;
  @include lg {
    font-size: 15px;
  }
  @include xl {
    font-size: 16px;
  }

  body {
    background-color: $background-color;
    margin: 0;

    .page-content {
      margin: 0 auto;
      max-width: 992px;
      padding: 0 20px;
    }
  }
}
</style>
