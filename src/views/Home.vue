<template>
  <section>
    <div class="parallax-container">
      <div class="parallax"></div>
      <h1>Joshua Richards</h1>
      <h4>Full Stack Developer</h4>
    </div>
    <section class="intro">
      <p>
        I am a full stack developer with experience ranging from web APIs to embedded systems.
        I have a passion for learning new technologies to implement projects both effectively and efficiently.
      </p>
    </section>
    <section id="indexNav">
      <div class="iconContainer">
        <router-link class="waves-effect waves-light btn" to="/experience">
          <h5>Experience</h5>
          <i class="large material-icons">work</i>
        </router-link>
      </div>
      <div class="iconContainer">
        <router-link class="waves-effect waves-light btn" to="/projects">
          <h5>Projects</h5>
          <i class="large material-icons">laptop</i>
        </router-link>
      </div>
      <div class="iconContainer">
        <router-link class="waves-effect waves-light btn" to="/resume">
          <h5>Resume</h5>
          <i class="large material-icons">assignment</i>
        </router-link>
      </div>
    </section>
  </section>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style lang="scss" scoped>
.page-content {
  padding: 0;
  max-width: none;
  .parallax-container {
    position: relative;
    overflow: hidden;
    width: 100%;
    height: 350px;
    @include sm {
      height: 450px;
    }
    @include xl {
      height: 500px;
    }
    .parallax {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      z-index: -1;
      background-image: url("../assets/blue-bright-clouds.jpg");
      background-attachment: fixed;
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
    }
    h1 {
      color: #fff;
      text-align: center;
      font-size: 3rem;
      font-weight: 300;
      margin: 6rem 0 0;
      @include sm {
        font-size: 5rem;
      }
      @include xl {
        font-size: 6rem;
      }
    }
    h4 {
      color: #fff;
      text-align: center;
      font-size: 1.5rem;
      font-weight: 300;
      margin: .6rem 0 0;
      @include sm {
        font-size: 2rem;
      }
    }
  }
  .intro {
    background-color: $background-intro;
    p {
      margin: 0 auto;
      font-size: 1.2rem;
      text-align: center;
      max-width: 1020px;
      padding: 40px 20px;
      @include sm {
        font-size: 1.5rem;
      }
    }
  }
}
</style>