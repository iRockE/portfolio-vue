<template>
  <footer class="page-footer">
    <div class="container">
      <div class="right-col">
        <h5>Contact</h5>
        <ul>
          <li>
            <p class="grey-text text-lighten-4">Email: jmrichards96@gmail.com</p>
          </li>
          <li>
            <p class="grey-text text-lighten-4">Phone: (860) 951-6629</p>
          </li>
        </ul>
      </div>
      <div class="left-col">
        <h5>Social</h5>
        <ul>
          <li><a class="social-link" target="_blank" href="https://www.linkedin.com/in/j-richards/">
            <img src="@/assets/linkedin.png" alt="Linkedin" />
          </a></li>
          <li><a class="social-link" target="_blank" href="https://github.com/iRockE">
            <img src="@/assets/github.png" alt="GitHub" />
          </a></li>
        </ul>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">© 2018 Joshua Richards - All Rights Reserved</div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'AppFooter'
}
</script>

<style lang="scss" scoped>
.page-footer {
    padding-top: 30px;
    color: #fff;
    background-color: #546e7a;
    & > .container {
      margin-bottom: 20px;
      max-width: 992px;
      &:after {
        content: "";
        display: table;
        clear: both;
      }
      .right-col {
        float: left;
        box-sizing: border-box;
        padding: 0 .75rem;
        min-height: 1px;
        width: 100%;
        margin-left: auto;
        left: auto;
        right: auto;
        @include md {
          width: 50%;
        }
      }
      .left-col {
        float: left;
        box-sizing: border-box;
        padding: 0 .75rem;
        min-height: 1px;
        width: 100%;
        margin-left: auto;
        left: auto;
        right: auto;
        @include md {
          margin-left: 20%;
          width: 30%;
        }
      }
    }
    h5 {
      font-size: 1.64rem;
      font-weight: 400;
      margin: 0 0 .4rem 0;
    }
    ul {
      padding-left: 0;
      list-style-type: none;
      li {
        list-style-type: none;
      }
    }
    .footer-copyright {
      overflow: hidden;
      min-height: 50px;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 10px 0px;
      color: rgba(255,255,255,0.8);
      background-color: rgba(51,51,51,0.08);
      box-sizing: border-box;
    }
    .social-link {
      display: block;
      height: 40px;
      width: 40px;
      margin: .5em 0;
      color: #eee;
      img {
        width: 40px;
      }
    }
}
.container {
  margin: 0 auto;
  max-width: 1020px;
  width: 90%;
}
</style>