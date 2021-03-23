<template>
    <NavBar />
    <router-view/>
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
  font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif;
  font-weight: normal;
  color: rgba(0,0,0,0.87);

  body {
    background-color: $background-color;
    margin: 0;
  }
}
</style>
