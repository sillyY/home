<template>
  <header>
    <div class="container">
      <div class="nav-brand">
        <a href="">
          <h1>
            <img
              class="nes-avatar is-rounded is-large"
              alt="Avatar"
              src="../assets/avatar.jpeg"
              style="image-rendering: pixelated"
            />
            SillyY
          </h1>
        </a>
        <p class="nes-text">
          <span class="lang-zh">笨鸟先飞，勤能补拙 </span>
          <span>Industry makes up for clumsiness</span>
        </p>
      </div>
      <div class="social-button">
        Share on SNS
        <div class="share">
          <a href="https://github.com/sillyY" target="_blank"
            ><im class="nes-icon github"></im
          ></a>
        </div>
      </div>
    </div>
  </header>
  <main>
    <div class="container">
      <section class="topic">
        <h2 id="about">
          <a href="#about">#</a>
          About
        </h2>
        <p>Hello, I am SillyY.</p>
      </section>
      <section class="topic">
        <h2 id="blog">
          <a href="#about">#</a>
          Blog
        </h2>
        <a href="https://sillyy.github.io/" class="nes-badge">
          <span class="is-success">Click Me</span>
        </a>
      </section>
      <section class="topic">
        <h2 id="repository">
          <a href="#repository">#</a>
          Repository
        </h2>
        <div class="repo-container">
          <section class="nes-container is-dark repo-card">
            <div class="avatar">
              <img
                class="nes-avatar is-large"
                alt="Avatar"
                src="../assets/facility.png"
                style="image-rendering: pixelated"
              />
            </div>
            <div class="profile">
              <h4 class="name">facility</h4>
              <p class="lang-zh">
                VSCode extension that helps rapid development
              </p>
              <div>
                <a
                  href="https://github.com/sillyY/facility"
                  target="_blank"
                  rel="noopener"
                  aria-label="github"
                  ><i class="nes-icon github"></i
                ></a>
                <a
                  href="https://marketplace.visualstudio.com/items?itemName=sillyy.facility"
                  class="nes-badge is-splited"
                >
                  <span class="name">version</span>
                  <span class="version">0.3.3</span>
                </a>
              </div>
            </div>
          </section>
          <section class="nes-container is-dark repo-card">
            <div class="avatar">
              <img
                class="nes-avatar is-large"
                alt="Avatar"
                src="../assets/default.svg"
                style="image-rendering: pixelated"
              />
            </div>
            <div class="profile">
              <h4 class="name">ideploy</h4>
              <p class="lang-zh">Project release command line tool</p>
              <div>
                <a
                  href="https://github.com/sillyY/ideploy"
                  target="_blank"
                  rel="noopener"
                  aria-label="github"
                  ><i class="nes-icon github"></i
                ></a>
              </div>
            </div>
          </section>
          <section class="nes-container is-dark repo-card">
            <div class="avatar">
              <img
                class="nes-avatar is-large"
                alt="Avatar"
                src="../assets/default.svg"
                style="image-rendering: pixelated"
              />
            </div>
            <div class="profile">
              <h4 class="name">Reading</h4>
              <p class="lang-zh">追书神器API</p>
              <div>
                <a
                  href="https://github.com/sillyY/Reading"
                  target="_blank"
                  rel="noopener"
                  aria-label="github"
                  ><i class="nes-icon github"></i
                ></a>
              </div>
            </div>
          </section>
          <section class="nes-container is-dark repo-card">
            <div class="avatar">
              <img
                class="nes-avatar is-large"
                alt="Avatar"
                src="../assets/default.svg"
                style="image-rendering: pixelated"
              />
            </div>
            <div class="profile">
              <h4 class="name">vuepress-plugin-code-segment</h4>
              <p class="lang-zh">vuepress code segment plugin</p>
              <div>
                <a
                  href="https://github.com/sillyY/vuepress-plugin-code-segment"
                  target="_blank"
                  rel="noopener"
                  aria-label="github"
                  ><i class="nes-icon github"></i
                ></a>
              </div>
            </div>
          </section>
        </div>
      </section>
    </div>
  </main>
  <footer>
    <p>
      Designed &amp; Powerd by
      <a href="/">sillyy</a>
      <br />Copyright© 2020 sillyy
      <br />
      <a href="http://beian.miit.gov.cn" target="_blank" rel="nofollow"
        ><span class="lang-zh">浙备</span>20010024<span class="lang-zh"
          >号</span
        ></a
      >
    </p>
  </footer>
</template>
<script>
export default {
  name: "Home",
  data() {
    return {
      cardStyle: {
        width: "200px",
        minHeight: "200px",
      },
      repositories: [
        {
          label: "Reading",
          content: "追书神器API",
          url: "https://github.com/sillyY/Reading",
        },
        {
          label: "vuepress-plugin-code-segment",
          content: "vuepress plugin",
          url: "https://github.com/sillyY/vuepress-plugin-code-segment",
        },
        {
          label: "diff-dir-file",
          content: "directory compare and show the difference of files",
          url: "https://github.com/sillyY/diff-dir-file",
        },
        {
          label: "facility",
          content: "A VSCode extension that helps rapid development",
          url: "https://github.com/sillyY/facility",
        },
      ],
    };
  },
  mounted() {},
  methods: {},
};
</script>
<style lang="scss" scope>
header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 9;
  border-bottom: 4px solid #d3d3d3;
  background-color: white;
  .container {
    display: flex;
    align-items: baseline;
    max-width: 980px;
    margin: 0 auto;
    padding-top: 1rem;
    transition: all 0.2s ease;
    .nav-brand {
      margin-right: auto;
      a {
        color: #212529;
        text-decoration: none;
        img {
          position: relative;
          display: inline-block;
          width: 60px;
          height: 60px;
        }
      }
    }
  }
}
main {
  max-width: 980px;
  margin: 0 auto;
  margin-top: 150px;
  .container {
    margin-bottom: 4rem;
    .topic {
      margin-bottom: 3rem;
      .repo-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        .repo-card {
          display: flex;
          padding: 1rem 1.5rem;
          width: 470px;
          margin-bottom: 2rem;
          .profile {
            margin-left: 1.5rem;
            & > .name {
              font-size: 20px;
            }

            .nes-badge {
              width: 15.5em;
              margin-left: 20px;
              .name {
                position: absolute;
                top: 0;
                width: 50%;
                color: #fff;
                text-align: center;
                background-color: #61a1ff;
                left: 0;
                box-shadow: 0 0.5em #61a1ff, 0 -0.5em #61a1ff, 0 0 #61a1ff,
                  -0.5em 0 #61a1ff;
              }
              .version {
                background-color: #3a8aff;
                position: absolute;
                top: 0;
                width: 50%;
                color: #fff;
                text-align: center;
                background-color: #3a8aff;
                right: 0;
                box-shadow: 0 0.5em#3a8aff, 0 -0.5em#3a8aff, 0.5em 0 #3a8aff,
                  0 0 #3a8aff;
              }
            }
          }
        }
      }
    }
  }
}
footer {
  flex: 1;
  text-align: center;
}
.lang-zh {
  font-family: "Zpix";
  vertical-align: top;
}
</style>