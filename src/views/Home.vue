<template>
  <section>
    <div class="parallax-container">
      <div class="parallax"></div>
      <h1>Joshua Richards</h1>
      <h4>Full Stack Developer</h4>
    </div>
    <section class="intro">
      <p>
        I am a full stack (primarily front-end) developer with experience ranging from web APIs to embedded systems. I have a passion for learning new technologies to implement projects both effectively and efficiently.
      </p>
    </section>
    <section class="indexNav">
      <div class="iconContainer">
        <router-link to="/experience">
          <h5>Experience</h5>
          <i class="material-icons">work</i>
        </router-link>
      </div>
      <div class="iconContainer">
        <router-link to="/projects">
          <h5>Projects</h5>
          <i class="material-icons">laptop</i>
        </router-link>
      </div>
      <div class="iconContainer">
        <router-link to="/resume">
          <h5>Resume</h5>
          <i class="material-icons">assignment</i>
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
  .indexNav {
    padding: 80px 0;
    text-align: center;
    .iconContainer {
      padding: 20px 30px;
      @include md {
        display: inline-block;
      }
      @include xl {
        padding: 20px 50px;
      }
      a {
        border: none;
        border-radius: 2px;
        padding: 0 16px;
        text-transform: uppercase;
        outline: 0;
        text-align: center;
        letter-spacing: .5px;
        text-decoration: none;
        color: #fff;
        position: relative;
        cursor: pointer;
        display: inline-block;
        overflow: hidden;
        user-select: none;
        -webkit-tap-highlight-color: transparent;
        vertical-align: middle;
        z-index: 1;
        width: 180px;
        height: auto;
        -webkit-transition: 0.4s ease;
        transition: 0.4s ease;
        background-color: $button-color;
        box-sizing: border-box;
        box-shadow: 0 2px 2px 0 rgb(0 0 0 / 14%), 0 3px 1px -2px rgb(0 0 0 / 12%), 0 1px 5px 0 rgb(0 0 0 / 20%);
        &:hover {
          background-color: $button-hover-color;
          box-shadow: 0 3px 3px 0 rgb(0 0 0 / 14%), 0 1px 7px 0 rgb(0 0 0 / 12%), 0 3px 1px -1px rgb(0 0 0 / 20%);
          @include md {
            -webkit-transform: scale(1.08);
            transform: scale(1.08);
          }
        }
        h5 {
          font-size: 1.64rem;
          font-weight: 400;
          line-height: 110%;
          margin: 1rem 0 .4rem 0;
        }
        i {
          font-size: 6rem;
          line-height: 1;
          margin-bottom: .5rem;
        }
      }
    }
  }
}
</style>