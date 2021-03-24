<template>
  <section>
    <NavBreadcrumb :trail="['Home', 'Resume']" />
    <h1>Resume</h1>
    <LinkButton :href="sourcePDF" download>Download PDF</LinkButton>
    <section class="body-section">
      <h2>Summary</h2>
      <p>Software Engineer with development experience ranging from web APIs to embedded systems, driven to work 
        individually or in a team environment to implement projects both effectively and efficiently.</p>
    </section>
    <section class="body-section">
      <h2>Skills</h2>
      <h5>Technologies</h5>
      <p>JavaScript/TypeScript, ES6, Node.js, CSS, HTML, C#, C++, Git</p>
      <h5>Other</h5>
      <ul>
        <li>Ability to handle numerous responsibilities and desire to learn required skills</li>
        <li>Experience working in an agile development environment, implementing project features over a 
          series of iterations within a release cycle</li>
      </ul>
    </section>
    <section class="body-section">
      <h2>Experience</h2>
      <div class="resumeExperience">
        <h3>Carrier Global Corporation</h3>
        <h4>Pittsford, NY <span class="right">Dec 15, 2018 – Present</span></h4>
        <h5>Software Engineer</h5>
        <p>Responsible for the development of a web-based video streaming interface for security
          applications (with technologies including ES6, TypeScript, Node.js, RxJS, WebSockets).</p>
        <p>- Technical lead of the project from January, 2020 to August, 2020. </p>
        <p>Responsible for some development on one of the applications that uses the streaming
          interface mentioned above (with technologies including Node.js, React, Redux).</p>
        <p>Utilizing services such as Rally, GitHub, Jenkins (CI/CD), and Azure.</p>
      </div>
      <div class="resumeExperience">
        <h3>UTC Fire & Security Americas Corp</h3>
        <h4>Pittsford, NY <span class="right">Aug 27, 2018 – Dec 14, 2018</span></h4>
        <h5>Software Engineering Intern</h5>
        <p>Responsible for the development of a web-based security-driven video streaming interface (with technologies including ES6, TypeScript, Node.js, RxJS).</p>
      </div>
      <div class="resumeExperience">
        <h3>Gerber Technology</h3>
        <h4>Tolland, CT <span class="right">June 4, 2018 – Aug 10, 2018</span></h4>
        <h5>Software Engineering Intern</h5>
        <p>Responsible for the development of a variety of safety enhancements to a material spreading system (with C++).</p>
      </div>
      <div class="resumeExperience">
        <h3>EagleDream Technologies</h3>
        <h4>Rochester, NY <span class="right">Aug 28, 2017 – Dec 15, 2017</span></h4>
        <h5>Web Developer Co-op</h5>
        <p>Responsible for the development of various fit for purpose websites (with technologies including JavaScript, C#, SQL, CSS, Sass, WordPress, Shopify, PHP).</p>
      </div>
      <div class="resumeExperience">
        <h3>Gerber Technology</h3>
        <h4>Tolland, CT <span class="right">June 5, 2017 – Aug 11, 2017</span></h4>
        <h5>Software Engineering Intern</h5>
        <p>Responsible for the software development of a material cutting system’s label printing interface (with C# and XAML).</p>
      </div>
    </section>
    <section class="body-section">
      <h2>Education</h2>
      <h3>Rochester Institute of Technology</h3>
      <h4>Rochester, NY </h4>
      <h5 style="margin-bottom: .5rem;">Bachelor of Science in Game Design and Development</h5>
      <h5 style="margin-top: 0;">Minor in Computer Science</h5>
      <h4 class="gradDate">May 2019</h4>
      <ul>
        <li>GPA: 3.58</li>
      </ul>
      <h5>Courses</h5>
      <p>Introduction to Computer Science Theory, The Mechanics of Programming, Introduction to Software Engineering, 
        Concepts of Computer Systems, Analysis of Algorithms, Programming Language Concepts, Web Design & Implementation, 
        Rich Media Web App Dev I & II, Game Dev. and Algorithmic Problem Solving II, Interactive Media Development, 
        Data Structures & Algorithms for Games & Simulations I, Principles of Data Management</p>
    </section>
    <section class="body-section">
      <h2>Projects/Labs</h2>
      <ul class="projectList">
        <li>Developed TaskApp, a project task organizer, with technologies including Express, React, MongoDB, Redis, Gulp, and Sass.</li>
        <li>Developed qApp, a Node.js-driven rich web app where users can ask and answer questions.</li>
        <li>Developed the game Serpentine as an individual project with Unity and C# and published it to the Google Play store.</li>
        <li>As part of a team of five developed HealthNet, a management system for a collection of hospitals, employees, and patients with Django, a Python Web framework.</li>
      </ul>
    </section>
    <BackToTop />
  </section>
</template>

<script>
import NavBreadcrumb from "@/components/NavBreadcrumb";
import BackToTop from "@/components/BackToTop";
import LinkButton from "@/components/LinkButton";
import sourcePDF from "@/assets/Joshua_Richards_Resume.pdf";

export default {
  name: "Resume",
  components: {
    NavBreadcrumb,
    BackToTop,
    LinkButton
  },
  data() {
    return {
      sourcePDF: sourcePDF
    }
  }
};
</script>