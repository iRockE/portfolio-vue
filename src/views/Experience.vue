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
        connection protocols (WebSockets, WebRTC) in a number of browsers / operating systems.
        The interface is created with Node.js, utilizing technologies including ES6, TypeScript, and RxJS.</p>
      <p>Recently responsible for development work on one of the applications that uses the streaming
        interface mentioned above, which is composed of a number of microservices deployed through Azure. The front-end
        portion is built with technologies including Node.js, React, and Redux.</p>
      <h3>Software Engineering Co-op</h3>
      <h5>Aug 27, 2018 – Dec 14, 2018</h5>
      <p><i>Same as above</i></p>
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