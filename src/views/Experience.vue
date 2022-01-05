<template>
  <section>
    <NavBreadcrumb :trail="['Home', 'Experience']" />
    <h1>Experience</h1>
    <section class="body-section">
      <h2>Carrier Global Corporation</h2>
      <h4>Pittsford, NY</h4>
      <h3>Software Engineer</h3>
      <h5>Dec 15, 2018 – Present</h5>
      <p>As part of an international team, I am responsible for the development of a web-based security-driven
        video streaming interface. This requires support for multiple video codecs (H.264, MJPEG, etc.) and 
        connection protocols (WebSockets, WebRTC) in a number of browsers / operating systems. The interface supports 
        viewing live/recorded video, frame advancement, fast-forward/reverse, digital zoom, jumping to specific times, etc.
        The interface is created with Node.js, utilizing technologies including TypeScript/JavaScript, ES6, and RxJS.</p>
      <p>I also aid in the development of a SaaS security application that uses the streaming 
        interface mentioned above. The application is composed of a number of microservices deployed through Azure, and is focused
        on access control and video. The front-end services are built with technologies including JavaScript, Node.js, 
        React, Redux, Sass, i18next, and Ramda.</p>
      <p>I use services such as Rally (issue tracking), GitHub (version control), Jenkins (CI/CD), 
        Confluence (documentation), and Azure (cloud deployment/management).</p>
      <p>While continuing to act as an individual contributor on the above projects, I have served as a team lead 
        since May, 2021. Responsibilities include:</p>
      <ul>
        <li>Work with product management to plan features and define acceptance criteria</li>
        <li>Define all stories/tasks for a feature</li>
        <li>Run daily stand up and retrospective meetings</li>
        <li>Help team members resolve issues as they arise</li>
        <li>Give feature demos to product management and broader audiences</li>
      </ul>
      <h3>Software Engineering Co-op</h3>
      <h5>Aug 27, 2018 – Dec 14, 2018</h5>
      <p><i>See above</i></p>
    </section>
    <section class="body-section">
      <h2>Gerber Technology</h2>
      <h4>Tolland, CT</h4>
      <h3>Software Engineering Intern</h3>
      <h5>June 4, 2018 – Aug 10, 2018</h5>
      <p>In a team environment, I was responsible for the development of a variety of safety enhancements to 
        a material spreading system. The team consisted of a mechanical engineer, electrical engineer, and 
        software engineer (myself) among other roles. In addition to group milestones and presentations, 
        each member had objectives specific to their field. In coordination with the electrical engineer, I 
        was tasked with differentiating emergency stop locations on the spreading system so that they could 
        be meaningfully displayed to the operator. The software was created using the Microsoft Foundation 
        Class Library (with C++) as an addition to the system's existing software.</p>
      <h5>June 5, 2017 – Aug 11, 2017</h5>
      <p>In a group of three, I was responsible for the software development of a material cutting system’s 
        label printing interface (with C# and XAML). The group consisted of a mechanical engineer, electrical 
        engineer, and software engineer (myself). The interface was created in Windows Presentation Foundation 
        (with languages including C#, XAML, and SQL) as an addition to the system's existing interface.</p>
    </section>
    <section class="body-section">
      <h2>EagleDream Technologies</h2>
      <h4>Rochester, NY</h4>
      <h3>Web Developer Co-op</h3>
      <h5>Aug 28, 2017 – Dec 15, 2017</h5>
      <p>Individually and in a team environment, I was responsible for the development of various fit for 
        purpose websites catered to client needs. Objectives ranged from bug fixing to website redesigns and 
        ground-up development. Websites were developed with technologies including JavaScript, C#, SQL, CSS, 
        Sass, Razor, PHP, WordPress, Shopify, and Umbraco.</p>
    </section>
    <BackToTop />
  </section>
</template>

<script>
import NavBreadcrumb from "@/components/NavBreadcrumb";
import BackToTop from "@/components/BackToTop";

export default {
  name: "Experience",
  components: {
    NavBreadcrumb,
    BackToTop
  }
};
</script>

<style lang="scss" scoped>
ul {
  font-size: 1.1rem;
  margin-top: 0;
  margin-right: 20px;
}
</style>