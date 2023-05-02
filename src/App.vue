<template>
  <div class="wrapper">
    <div class="content">
      <header id="home">
        <div class="logo">
          <v-img :width="withLogo" :height="heigthLogo" :src="logo"></v-img>
        </div>
        <nav class="nav_header nav">
          <v-linc :href="'#home'" :msg="nameHome"></v-linc>
          <v-linc :href="'#abount'" :msg="nameAbount"></v-linc>
          <v-linc :href="'#tech_stack'" :msg="nameTechStack"></v-linc>
          <v-linc :href="'#project'" :msg="nameProjects"></v-linc>
          <v-linc :href="'#contact'" :msg="nameContact"></v-linc>
        </nav>
        <div class="header_icon">
          <v-img
            @click="test2"
            :width="withIcon"
            :height="heigthIcon"
            :src="githubIcon"
          ></v-img>
          <v-img
            :width="withIcon"
            :height="heigthIcon"
            :src="twitterIcon"
          ></v-img>
          <v-img
            :width="withIcon"
            :height="heigthIcon"
            :src="linkedinIcon"
          ></v-img>
        </div>
      </header>
      <main>
        <div class="content">
          <div id="abount" class="main_title">
            <div class="title">
              <v-text
                :color="colorD9D9D9"
                @click="test"
                :fontSize="fontSize58"
                :fontWeight="fontWeight700"
                :lineHeight="lineHeight70"
                :msg="msgH1"
              ></v-text>
            </div>
            <div class="main_foto">
              <v-img
                :width="withTitle"
                :height="heigthTitle"
                :src="imageTitle"
              ></v-img>
            </div>
          </div>
          <div id="tech_stack" class="mainTechStack">
            <div class="mainTechStackH2">
              <v-text :fontSize="fontSize48" :msg="msgH2"></v-text>
            </div>
            <div class="mainTechStackH3">
              <v-text
                :color="colorA7A7A7"
                :fontSize="fontSize32"
                :fontWeight="fontWeight400"
                :msg="msgH3"
              ></v-text>
            </div>
            <div class="stackImage">
              <v-img :src="htmlImage"></v-img>
              <v-img :src="cssImage"></v-img>
              <v-img :src="jsImage"></v-img>
              <v-img :src="reactImage"></v-img>
              <v-img :src="vectorImage"></v-img>
              <v-img :src="bootstrapImage"></v-img>
              <v-img :src="tailwindImage"></v-img>
              <v-img :src="sassImage"></v-img>
              <v-img :src="gitImage"></v-img>
              <v-img :src="greensockImage"></v-img>
              <v-img :src="vscodeImage"></v-img>
              <v-img :src="githubImage"></v-img>
            </div>
          </div>
          <div id="project" class="mainProject">
            <v-text :fontSize="fontSize48" :msg="nameTitleH2Project"></v-text>
            <v-text
              :color="colorA7A7A7"
              :fontSize="fontSize32"
              :fontWeight="fontWeight400"
              :msg="nameTitleH3Project"
            ></v-text>
            <div class="project_content">
              <div class="project">
                <div class="project_image">
                  <v-img
                    :width="withProject"
                    :height="heigthProject"
                    :src="project1"
                  ></v-img>
                </div>
                <div class="project_text_content">
                  <div class="project_title">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize28"
                      :fontWeight="fontWeight500"
                      :msg="nameProject1"
                    ></v-text>
                  </div>
                  <div class="project_text">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize18"
                      :fontWeight="fontWeight300"
                      :msg="textProject1"
                    ></v-text>
                  </div>
                  <div class="project_text2">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize16"
                      :fontWeight="fontWeight400"
                      :msg="techTextProject1"
                    ></v-text>
                  </div>
                  <div class="project_footer">
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsLinkChain"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLinkProject1"></v-linc>
                    </div>
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsGithub"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLink2Project1"></v-linc>
                    </div>
                  </div>
                </div>
              </div>
              <div class="project">
                <div class="project_image">
                  <v-img
                    :width="withProject"
                    :height="heigthProject"
                    :src="project2"
                  ></v-img>
                </div>
                <div class="project_text_content">
                  <div class="project_title">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize28"
                      :fontWeight="fontWeight500"
                      :msg="nameProject2"
                    ></v-text>
                  </div>
                  <div class="project_text">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize18"
                      :fontWeight="fontWeight300"
                      :msg="textProject2"
                    ></v-text>
                  </div>
                  <div class="project_text2">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize16"
                      :fontWeight="fontWeight400"
                      :msg="techTextProject2"
                    ></v-text>
                  </div>
                  <div class="project_footer">
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsLinkChain"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLinkProject2"></v-linc>
                    </div>
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsGithub"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLink2Project2"></v-linc>
                    </div>
                  </div>
                </div>
              </div>
              <div class="project">
                <div class="project_image">
                  <v-img
                    :width="withProject"
                    :height="heigthProject"
                    :src="project3"
                  ></v-img>
                </div>
                <div class="project_text_content">
                  <div class="project_title">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize28"
                      :fontWeight="fontWeight500"
                      :msg="nameProject3"
                    ></v-text>
                  </div>
                  <div class="project_text">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize18"
                      :fontWeight="fontWeight300"
                      :msg="textProject3"
                    ></v-text>
                  </div>
                  <div class="project_text2">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize16"
                      :fontWeight="fontWeight400"
                      :msg="techTextProject3"
                    ></v-text>
                  </div>
                  <div class="project_footer">
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsLinkChain"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLinkProject3"></v-linc>
                    </div>
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsGithub"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLink2Project3"></v-linc>
                    </div>
                  </div>
                </div>
              </div>
              <div class="project">
                <div class="project_image">
                  <v-img
                    :width="withProject"
                    :height="heigthProject"
                    :src="project4"
                  ></v-img>
                </div>
                <div class="project_text_content">
                  <div class="project_title">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize28"
                      :fontWeight="fontWeight500"
                      :msg="nameProject4"
                    ></v-text>
                  </div>
                  <div class="project_text">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize18"
                      :fontWeight="fontWeight300"
                      :msg="textProject4"
                    ></v-text>
                  </div>
                  <div class="project_text2">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize16"
                      :fontWeight="fontWeight400"
                      :msg="techTextProject4"
                    ></v-text>
                  </div>
                  <div class="project_footer">
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsLinkChain"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLinkProject4"></v-linc>
                    </div>
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsGithub"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLink2Project4"></v-linc>
                    </div>
                  </div>
                </div>
              </div>
              <div class="project">
                <div class="project_image">
                  <v-img
                    :width="withProject"
                    :height="heigthProject"
                    :src="project5"
                  ></v-img>
                </div>
                <div class="project_text_content">
                  <div class="project_title">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize28"
                      :fontWeight="fontWeight500"
                      :msg="nameProject5"
                    ></v-text>
                  </div>
                  <div class="project_text">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize18"
                      :fontWeight="fontWeight300"
                      :msg="textProject5"
                    ></v-text>
                  </div>
                  <div class="project_text2">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize16"
                      :fontWeight="fontWeight400"
                      :msg="techTextProject5"
                    ></v-text>
                  </div>
                  <div class="project_footer">
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsLinkChain"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLinkProject5"></v-linc>
                    </div>
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsGithub"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLink2Project5"></v-linc>
                    </div>
                  </div>
                </div>
              </div>
              <div class="project">
                <div class="project_image">
                  <v-img
                    :width="withProject"
                    :height="heigthProject"
                    :src="project6"
                  ></v-img>
                </div>
                <div class="project_text_content">
                  <div class="project_title">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize28"
                      :fontWeight="fontWeight500"
                      :msg="nameProject6"
                    ></v-text>
                  </div>
                  <div class="project_text">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize18"
                      :fontWeight="fontWeight300"
                      :msg="textProject6"
                    ></v-text>
                  </div>
                  <div class="project_text2">
                    <v-text
                      :color="colorA7A7A7"
                      :fontSize="fontSize16"
                      :fontWeight="fontWeight400"
                      :msg="techTextProject6"
                    ></v-text>
                  </div>
                  <div class="project_footer">
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsLinkChain"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLinkProject6"></v-linc>
                    </div>
                    <div class="project_footer_content">
                      <v-img
                        :width="withIcon"
                        :height="heigthIcon"
                        :src="iconsGithub"
                      ></v-img>
                      <v-linc :href="''" :msg="nameLink2Project1"></v-linc>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </main>
      <footer>
        <div id="contact" class="footer_contact">
          <div class="footer_logo_cotnent">
            <div class="footer_logo">
              <v-img
                :width="withLogo"
                :height="heigthLogo"
                :src="logoFooter"
              ></v-img>
            </div>
            <div class="footer_contacts">
              <v-text :fontSize="fontSize18" :msg="footerTel"></v-text>
              <v-text :fontSize="fontSize18" :msg="footerEmail"></v-text>
            </div>
          </div>
          <div class="footer_icon">
            <v-img
              :width="withIcon"
              :height="heigthIcon"
              :src="githubIcon"
            ></v-img>
            <v-img
              :width="withIcon"
              :height="heigthIcon"
              :src="twitterIcon"
            ></v-img>
            <v-img
              :width="withIcon"
              :height="heigthIcon"
              :src="linkedinIcon"
            ></v-img>
          </div>
        </div>
        <hr />
        <div class="footer_nav">
          <nav class="nav_footer nav">
            <v-linc :href="''" :msg="nameHome"></v-linc>
            <v-linc :href="''" :msg="nameAbount"></v-linc>
            <v-linc :href="''" :msg="nameTechStack"></v-linc>
            <v-linc :href="''" :msg="nameProjects"></v-linc>
            <v-linc :href="''" :msg="nameContact"></v-linc>
          </nav>
          <v-text
            :fontSize="fontSize18"
            :color="colorA7A7A7"
            :msg="footerText"
          ></v-text>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
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

import logo from "./assets/logo.png";
import githubIcon from "./assets/github.png";
import twitterIcon from "./assets/twitter.png";
import linkedinIcon from "./assets/linkedin.png";
import imageTitle from "./assets/imageTitle.png";
import project1 from "./assets/projects 1.png";
import project2 from "./assets/projects 2.png";
import project3 from "./assets/projects 3.png";
import project4 from "./assets/projects 4.png";
import project5 from "./assets/projects 5.png";
import project6 from "./assets/projects 6.png";
import iconsGithub from "./assets/iconsGithubFill.png";
import iconsLinkChain from "./assets/iconsLinkChain.png";
import logoFooter from "./assets/logoFooter.png";

import vImg from "./components/v-img.vue";
import vLinc from "./components/v-linc.vue";
import vText from "./components/v-text.vue";

export default {
  name: "App",
  components: {
    vImg,
    vLinc,
    vText,
  },
  methods: {
    test() {
      this.colorD9D9D9 = "red"
    },
    test2(){
      this.withIcon="35px"
      this.heigthIcon="35px"
      this.githubIcon="twitter"
    }
  },

  data() {
    return {
      nameHome: "Home",
      nameAbount: "Abount",
      nameTechStack: "Tech Stack",
      nameProjects: "Projects",
      nameContact: "Contact",
      withLogo: "97px",
      heigthLogo: "59px",
      withIcon: "30px",
      heigthIcon: "30px",
      msgH1: "Hi 👋, My name is Pavan MG I build things for web",
      withTitle: "349px",
      heigthTitle: "349px",
      msgH2: "My Tech Stack",
      msgH3: "Technologies I’ve been working with recently",
      nameTitleH2Project: "Projects",
      nameTitleH3Project: "Things I’ve built so far",
      
      withProject: "375px",
      heigthProject: "260px",

      colorD9D9D9: "#D9D9D9",
      colorDCCCCCC: "#D#CCCCCC",
      colorA7A7A7: "#A7A7A7",

      fontWeight700: "700",
      fontWeight500: "500",
      fontWeight400: "400",
      fontWeight300: "300",

      fontSize58: "58px",
      fontSize48: "48px",
      fontSize32: "32px",
      fontSize28: "28px",
      fontSize18: "18px",
      fontSize16: "16px",

      lineHeight70: "70px",
      lineHeight26: "26px",

      nameProject1: "Project Tile goes here",
      nameProject2: "Project Tile goes here",
      nameProject3: "Project Tile goes here",
      nameProject4: "Project Tile goes here",
      nameProject5: "Project Tile goes here",
      nameProject6: "Project Tile goes here",

      textProject1:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",
      textProject2:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",
      textProject3:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",
      textProject4:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",
      textProject5:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",
      textProject6:
        "This is sample project description random things are here in description This is sample project lorem ipsum generator for dummy content",

      techTextProject1: "Tech stack : HTML , JavaScript, SASS, React",
      techTextProject2: "Tech stack : HTML , JavaScript, SASS, React",
      techTextProject3: "Tech stack : HTML , JavaScript, SASS, React",
      techTextProject4: "Tech stack : HTML , JavaScript, SASS, React",
      techTextProject5: "Tech stack : HTML , JavaScript, SASS, React",
      techTextProject6: "Tech stack : HTML , JavaScript, SASS, React",

      withProjectIcon: "20px",
      heigthProjectIcon: "20px",

      nameLinkProject1: "Live Preview",
      nameLink2Project1: "View Code",
      nameLinkProject2: "Live Preview",
      nameLink2Project2: "View Code",
      nameLinkProject3: "Live Preview",
      nameLink2Project3: "View Code",
      nameLinkProject4: "Live Preview",
      nameLink2Project4: "View Code",
      nameLinkProject5: "Live Preview",
      nameLink2Project5: "View Code",
      nameLinkProject6: "Live Preview",
      nameLink2Project6: "View Code",

      footerTel: "+91 12345 09876",
      footerEmail: "info@example.com",
      footerText: "Designed and built by Pavan MG with Love & Coffee",

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
      project1,
      project2,
      project3,
      project4,
      project5,
      project6,
      iconsGithub,
      iconsLinkChain,
      logoFooter,
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
nav {
  max-width: 609px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin-left: 151px;
}
nav a:-webkit-any-link {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 26px;
  text-align: center;
  color: #a7a7a7;
  text-decoration: none;
}

main {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
}
.main_title {
  widows: 100%;
  display: flex;
  justify-content: space-between;
  margin-top: 270px;
  margin-bottom: 330px;
}
.title {
  width: 50%;
}

.mainTechStackH2 {
  text-align: center;
}
.mainTechStackH3,
.mainProject {
  text-align: center;
}
.project_content {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.project {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  max-width: 375px;
  width: 100%;
  background: #363636;
  box-shadow: 2px 2px 100px rgba(0, 0, 0, 0.2);
  border-radius: 20px;
  margin-bottom: 50px;
  margin-top: 50px;
}
.projecct_title {
  text-align: justify;
}

.project_text_content {
  padding: 0px 31px 0px 28px;
  text-align: justify;
}
.project_footer {
  display: flex;
  justify-content: space-between;
  width: 100%;
}
.project_footer_content {
  width: 50%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-right: 10%;
}
footer {
  max-width: 1193px;
  width: 100%;
  margin: 0 auto;
}
.footer_contact {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  margin-bottom: 20px;
}
.footer_contacts {
  display: flex;
  justify-content: space-between;
  width: 35%;
}
.footer_logo_cotnent {
  display: flex;
  justify-content: space-between;
  width: 85%;
}
.footer_nav {
  display: flex;
  justify-content: space-between;
  margin-top: 20px;
  align-items: center;
}
.nav_footer {
  margin: 0%;
}

.stackImage {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.stackImage div {
  margin: 50px 30px;
}
</style>
