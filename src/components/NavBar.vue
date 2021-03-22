<template>
  <nav>
    <div class="nav-wrapper">
      <router-link to="/" class="brand-logo"><img src="@/assets/logo.png" alt="Logo" ></router-link>
      <ul class="right hide-on-med-and-down">
        <li><router-link to="/experience">Experience</router-link></li>
        <li><router-link to="/projects">Projects</router-link></li>
        <li><router-link to="/resume">Resume</router-link></li>
      </ul>
      <ul id="nav-mobile" class="sidenav">
        <li><a href="/experience">Experience</a></li>
        <li><a href="/projects">Projects</a></li>
        <li><a href="/resume">Resume</a></li>
      </ul>
      <a href="#" data-target="nav-mobile" class="sidenav-trigger">
        <i class="material-icons">menu</i>
      </a>
    </div>
  </nav>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
