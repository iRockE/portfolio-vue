<template>
  <section>
    <NavBreadcrumb :trail="['Home', 'Projects']" />
    <h1>Projects</h1>
    <section class="body-section">
      <h2>Serpentine</h2>
      <h4>Unity, C#</h4>
      <a class="waves-effect waves-light btn"  target="_blank" href="https://play.google.com/store/apps/details?id=com.RockEStudios.Serpentine1">View Project</a>
    </section>
    <section class="body-section">
      <h2>TaskApp</h2>
      <h4>Node.js, Express, React, MongoDB, Redis, Sass, Gulp</h4>
    </section>
    <section class="body-section">
      <h2>qApp</h2>
      <h4>Node.js</h4>
      <a class="waves-effect waves-light btn"  target="_blank" href="https://qapp-application.herokuapp.com/">View Project</a>
    </section>
    <BackToTop />
  </section>
</template>

<script>
import NavBreadcrumb from "@/components/NavBreadcrumb";
import BackToTop from "@/components/BackToTop";

export default {
  name: "Projects",
  components: {
    NavBreadcrumb,
    BackToTop
  }
};
</script>