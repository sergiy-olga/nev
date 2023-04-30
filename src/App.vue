<template>
  <div>
    <div id="Home" class="content">
      <header class="header">
        <div class="header_logo">
          <v-logo :src="logo"></v-logo>
        </div>
        <div class="nav_icon">
          <div class="nav">
            <v-link
              v-bind="config"
              v-for="config in list"
              :key="config.msg"
            ></v-link>
          </div>
          <div class="header_icon">
            <v-HeaderIcon :src="githubIcon"></v-HeaderIcon>
            <v-HeaderIcon :src="twitterIcon"></v-HeaderIcon>
            <v-HeaderIcon :src="linkedinIcon"></v-HeaderIcon>
          </div>
        </div>
      </header>
      <main class="main">
        <div class="main_title">
          <div class="main_section">
            <v-MainH1></v-MainH1>
          </div>
          <div>
            <v-imageTitle :src="imageTitle"></v-imageTitle>
          </div>
        </div>
        <div id="Tech_Stack" class="content tech-steck">
          <v-titleH2H3 :titleH2="h2Stack" :titleH3="h3Stack"></v-titleH2H3>
          <div class="icon_content">
            <div class="icon">
              <v-image :src="htmlImage"></v-image>
              <v-image :src="cssImage"></v-image>
              <v-image :src="jsImage"></v-image>
              <v-image :src="reactImage"></v-image>
              <v-image :src="vectorImage"></v-image>
              <v-image :src="bootstrapImage"></v-image>
            </div>
            <div class="icon">
              <v-image :src="tailwindImage"></v-image>
              <v-image :src="sassImage"></v-image>
              <v-image :src="gitImage"></v-image>
              <v-image :src="greensockImage"></v-image>
              <v-image :src="vscodeImage"></v-image>
              <v-image :src="githubImage"></v-image>
            </div>
          </div>
        </div>
        <div id="Projects">
          <v-titleH2H3
            :titleH2="h2Projects"
            :titleH3="h3Projects"
          ></v-titleH2H3>
          <div class="projects">
            <v-Projects
              :src="project1"
              :src2="iconsGithub"
              :src1="iconsLinkChain"
              :msgH4="msgH4"
              :msgText="msgText"
              :msgP="msgP"
              :href="'#Projects'"
              :msg="msg"
              :msg1="msg1"
            >
            </v-Projects>
            <v-Projects
              :src="project2"
              :src2="iconsGithub"
              :src1="iconsLinkChain"
              :msgH4="msgH4"
              :msgText="msgText"
              :msgP="msgP"
              :href="'#Projects'"
              :msg="msg"
              :msg1="msg1"
            >
            </v-Projects>
            <v-Projects
              :src="project3"
              :src2="iconsGithub"
              :src1="iconsLinkChain"
              :msgH4="msgH4"
              :msgText="msgText"
              :msgP="msgP"
              :href="'#Projects'"
              :msg="msg"
              :msg1="msg1"
            >
            </v-Projects>
            <v-Projects
              :src="project4"
              :src2="iconsGithub"
              :src1="iconsLinkChain"
              :msgH4="msgH4"
              :msgText="msgText"
              :msgP="msgP"
              :href="'#Projects'"
              :msg="msg"
              :msg1="msg1"
            >
            </v-Projects>
            <v-Projects
              :src="project5"
              :src2="iconsGithub"
              :src1="iconsLinkChain"
              :msgH4="msgH4"
              :msgText="msgText"
              :msgP="msgP"
              :href="'#Projects'"
              :msg="msg"
              :msg1="msg1"
            >
            </v-Projects>
            <v-Projects
              :src="project6"
              :src2="iconsGithub"
              :src1="iconsLinkChain"
              :msgH4="msgH4"
              :msgText="msgText"
              :msgP="msgP"
              :href="'#Projects'"
              :msg="msg"
              :msg1="msg1"
            >
            </v-Projects>
          </div>
        </div>
      </main>
      <footer id="Contact">
        <div class="footer_header">
          <v-logo :src="logoFooter"></v-logo>
          <v-FooterTel :msg="vFooterTel" :msg1="vFooterEmail"></v-FooterTel>
          <div class="footer_icon">
            <v-HeaderIcon :src="githubIcon"></v-HeaderIcon>
            <v-HeaderIcon :src="twitterIcon"></v-HeaderIcon>
            <v-HeaderIcon :src="linkedinIcon"></v-HeaderIcon>
          </div>
        </div>
        <div class="footer_footer">
          <div class="nav">
            <v-link
              v-bind="config"
              v-for="config in list"
              :key="config.msg"
            ></v-link>
          </div>
          <v-FooterText :msg="vFooterText"></v-FooterText>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
import vImage from "./components/v-image.vue";
import htmlImage from "./assets/html.png";
import cssImage from "./assets/css.png";
import jsImage from "./assets/js.png";
import reactImage from "./assets/react.png";
import vectorImage from "./assets/Vector.png";
import bootstrapImage from "./assets/bootstrap.png";
import tailwindImage from "./assets/tailwind.png";
import sassImage from "./assets/sass.png";
import gitImage from "./assets/git.png";
import greensockImage from "./assets/greensock.png";
import vscodeImage from "./assets/vscode.png";
import githubImage from "./assets/github.png";
import vLogo from "./components/v-logo.vue";
import logo from "./assets/logo.png";
import vHeaderIcon from "./components/v-HeaderIcon.vue";
import githubIcon from "./assets/github.png";
import twitterIcon from "./assets/twitter.png";
import linkedinIcon from "./assets/linkedin.png";
import vImageTitle from "./components/v-imageTitle.vue";
import imageTitle from "./assets/50353683.png";
import vLink from "./components/v-link.vue";
import vMainH1 from "./components/v-MainH1.vue";
import vTitleH2H3 from "./components/v-titleH2H3.vue";

import vProjects from "./components/v-Projects.vue";
import project1 from "./assets/projects 1.png";
import project2 from "./assets/projects 2.png";
import project3 from "./assets/projects 3.png";
import project4 from "./assets/projects 4.png";
import project5 from "./assets/projects 5.png";
import project6 from "./assets/projects 6.png";
import iconsGithub from "./assets/iconsGithubFill.png";
import iconsLinkChain from "./assets/iconsLinkChain.png";
import logoFooter from "./assets/logoFooter.png";

import vFooterTel from "./components/v-FooterTel.vue";
import vFooterText from "./components/v-FooterText.vue";
export default {
  name: "App",
  components: {
    vImage,
    vLogo,
    vHeaderIcon,
    vImageTitle,
    vLink,
    vMainH1,
    vTitleH2H3,
    vProjects,
    vFooterTel,
    vFooterText,
  },
  data() {
    return {
      htmlImage,
      cssImage,
      jsImage,
      reactImage,
      vectorImage,
      bootstrapImage,
      tailwindImage,
      sassImage,
      gitImage,
      greensockImage,
      vscodeImage,
      githubImage,
      logo,
      githubIcon,
      twitterIcon,
      linkedinIcon,
      imageTitle,
      list: [
        {
          href: "#Home",
          msg: "Home",
        },
        {
          href: "#Abount",
          msg: "Abount",
        },
        {
          href: "#Tech_Stack",
          msg: "Tech Stack",
        },
        {
          href: "#Projects",
          msg: "Projects",
        },
        {
          href: "#Contact",
          msg: "Contact",
        },
      ],
      h2Stack: "My Tech Stack",
      h3Stack: "Technologies I’ve been working with recently",
      h2Projects: "Projects",
      h3Projects: "Things I’ve built so far",
      msgH4: "Project Tile goes here",
      msgText:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",
      msgP: "Tech stack : HTML , JavaScript, SASS, React",
      msg: "Live Preview",
      msg1: "View Code",
      project1,
      project2,
      project3,
      project4,
      project5,
      project6,
      iconsGithub,
      iconsLinkChain,
      logoFooter,
      vFooterTel: "+91 12345 09876",
      vFooterEmail: "info@example.com",
      vFooterText: "Designed and built by Pavan MG with Love & Coffee",
    };
  },
};
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #191919;
}
.icon_content {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
}
.icon {
  display: flex;
  justify-content: space-between;
  background: #191919;
}

.icon:nth-child(1) {
  margin-bottom: 83px;
}
.content {
  max-width: 1600px;
  width: 100%;
  background: #191919;
  margin: 0 auto;
  padding-top: 41px;
  padding-bottom: 40px;
}
header {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header_icon,
.footer_icon {
  display: flex;
  width: 130px;
  justify-content: space-between;
}
.nav {
  max-width: 609px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin-right: 51px;
}

.nav_icon {
  display: flex;
  max-width: 790px;
  width: 100%;
}

main {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
}
.main_title {
  display: flex;
  justify-content: space-between;
  margin-top: 270px;
  margin-bottom: 330px;
}
.projects {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
footer {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
}
.footer_header {
  display: flex;
  justify-content: space-between;
  width: 100%;
  align-items: center;
  margin-bottom: 50px;
}
.footer_footer{
  display: flex;
  justify-content: space-between;
  width: 100%;
  align-items: center;
}
</style>
