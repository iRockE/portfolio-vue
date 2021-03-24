<template>
    <NavBar />
    <router-view v-slot="{ Component }" class="page-content">
      <transition name="router-fade" mode="out-in">
        <component :is="Component" />
      </transition>
    </router-view>
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
      box-sizing: border-box;

      h1 {
        text-align: center;
        margin: 1rem 0 5rem;
        font-weight: 100;
        font-size: 4.6rem;
        @include sm {
          font-size: 6rem;
        }
      }
    }
  }
}

/*#region Transitions*/
.router-fade-enter-active {
  transition: opacity .3s;
}
.router-fade-leave-active {
  transition: opacity .1s;
}
.router-fade-enter-from,
.router-fade-leave-to {
  opacity: 0;
}
/*#endregion*/
</style>
