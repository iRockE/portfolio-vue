<template>
  <section>
    <NavBreadcrumb :trail="['Home', 'Projects']" />
    <h1>Projects</h1>
    <section class="body-section">
      <h2>Digital Resume</h2>
      <h4>Node.js, Vue 3, Vue Router, Sass, Webpack</h4>
    </section>
    <section class="body-section">
      <h2>TaskApp</h2>
      <h4>Node.js, Express, React, MongoDB, Redis, Sass, Gulp</h4>
    </section>
    <section class="body-section">
      <h2>Serpentine</h2>
      <h4>Unity, C#</h4>
      <LinkButton link="https://play.google.com/store/apps/details?id=com.RockEStudios.Serpentine1">View Project</LinkButton>
    </section>
    <section class="body-section">
      <h2>qApp</h2>
      <h4>Node.js</h4>
      <LinkButton link="https://qapp-application.herokuapp.com/">View Project</LinkButton>
    </section>
    <BackToTop />
  </section>
</template>

<script>
import NavBreadcrumb from "@/components/NavBreadcrumb";
import BackToTop from "@/components/BackToTop";
import LinkButton from "@/components/LinkButton";

export default {
  name: "Projects",
  components: {
    NavBreadcrumb,
    BackToTop,
    LinkButton
  }
};
</script>