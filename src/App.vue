<template>
  <header class="regular">
    <img src="./assets/logo_1.svg">
    <div class="header__menu">
      <a href="#">Features</a>
      <a href="#">Pricing</a>
      <a href="#">Blog</a>
      <a href="#">Docs</a>
      <a href="#">Changelog</a>
      <a href="#">We're hiring</a>
    </div>
    <div class="login">login</div>
  </header>
  <main-component/>
  <div class="article">
    <span class="bold">Select project,</span>
    <span class="regular">
      check dependencies, checkout branch, view<br>
      readme.txt, install tools, run build, run test,
    </span>
    <span class="bold">start coding.</span>
  </div>
  <about-component/>
  <secure-component/>
  <users-component/>
  <div class="companies__list">
    <img src="./assets/lb_gitlab.svg">
    <img src="./assets/lb_freecodecamp.svg">
    <img src="./assets/lb_dwave.svg">
    <img src="./assets/lb_google.svg">
    <img src="./assets/lb_amazon.svg">
    <img src="./assets/lb_facebook.svg">
    <img src="./assets/lb_uber.svg">
    <img src="./assets/lb_openai.svg">
    <img src="./assets/lb_intel.svg">
    <img src="./assets/lb_theia.svg">
    <img src="./assets/lb_code.svg">
    <img src="./assets/lb_4geeks.svg">
  </div>
  <start-component/>
  <footer>
    <div class="footer_menu regular">
      <ul>
        <li class="bold"><a href="#">GitPod</a></li>
        <li><a href="#">Home</a></li>
        <li><a href="#">Features</a></li>
        <li><a href="#">Pricing</a></li>
        <li><a href="#">Changelog</a></li>
        <li><a href="#">Self-Hosted</a></li>
        <li><a href="#">Gitpod vs GitHub<br>
          Codespaces</a></li>
        <li><a href="#">Status</a></li>
      </ul>
      <ul>
        <li class="bold"><a href="#">Developer</a></li>
        <li><a href="#">Getting started</a></li>
        <li><a href="#">Screencast</a></li>
        <li><a href="#">Blog</a></li>
        <li><a href="#">Documentation</a></li>
        <li><a href="#">Report a bug</a></li>
        <li><a href="#">Community</a></li>
      </ul>
      <ul>
        <li class="bold"><a href="#">Company</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Careers</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">Media Kit</a></li>
      </ul>
      <ul>
        <li class="bold"><a href="#">Legal</a></li>
        <li><a href="#">Imprint</a></li>
        <li><a href="#">Terms of Service</a></li>
        <li><a href="#">Privacy Policy</a></li>
      </ul>
    </div>
    <div class="footer_copyright">
      <div class="copyright">
        <img src="../src/assets/logo_2.svg">
        Copyright © 2021 Gitpod
      </div>
      <div class="media">
        <img src="../src/assets/ic_twitter_orange.svg">
        <img src="../src/assets/ic_github_orange.svg">
        <img src="../src/assets/ic_chat_orange.svg">
      </div>
    </div>

  </footer>
</template>

<script>

import MainComponent from "@/components/MainComponent";
import AboutComponent from "@/components/AboutComponent";
import SecureComponent from "@/components/SecureComponent";
import UsersComponent from "@/components/UsersComponent";
import StartComponent from "@/components/StartComponent";
export default {
  name: 'App',
  components: {
    StartComponent,
    UsersComponent,
    SecureComponent,
    AboutComponent,
    MainComponent
  }
}
</script>

<style>
@font-face {
  font-family: 'Roboto';
  src: url('./assets/Roboto-Regular.ttf') format('truetype');
  font-weight: 400;
}
@font-face {
  font-family: 'Roboto';
  src: url('./assets/Roboto-Bold.ttf') format('truetype');
  font-weight: 700;
}
:root{
  --white: #F5F3F4;
  --black: #12100C;
  --grey: #6A6766;
  --ligh-grey: #999795;
  --yellow: #FFAE33;
  --orange: #FC6D26;
  --peach: #FFE4BC;
  --pink: #FFB0AE;
  --blue: #2684FF;
}
.regular{
  font-family: Roboto,serif;
  font-weight: 400;
  line-height: 150%;
}
.bold{
  font-family: Roboto,serif;
  font-weight: 700;
  line-height: 110%;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  color: var(--black);
  list-style-type: none;
}
body{
  background: var(--white);
}
header{
  display: flex;
  justify-content: space-between;
  margin: 32px 20px 32px 20px;
  align-items: center;
}
.header__menu{
  display: flex;
  gap: 48px;
}
.login{
  height: 32px;
  width: 80px;
  background: var(--black);
  color: var(--white);
  border-radius: 12px;
  text-align: center;
  line-height: 32px;
  transition: 0.15s ease-in-out;
}
.login:hover{
  background: var(--yellow);
}
.article{
  display: flex;
  flex-flow: column;
  align-items: center;
  font-size: 54px;
}
.article .regular{
  color: var(--ligh-grey);
  text-decoration: line-through;
  text-decoration-thickness: 4px ;
}
.companies__list{
  display: flex;
  flex-flow: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 24px;
}
.companies__list{
  flex-basis: calc(100% / 7);
}
footer{
  display: flex;
  flex-flow: column;
  align-items: center;
  gap:47px;
  width: 100%;
  padding: 0 230px;
  align-self: center;
}
.footer_menu{
  width: 100%;
  display: flex;
  flex-flow: row;
  flex-wrap: wrap;
  justify-content: space-around;
}
.footer_menu ul{
  display: flex;
  flex-flow: column;
  gap: 8px;
}
.footer_copyright{
  display: flex;
  flex-flow: row;
  justify-content: space-between;
  width: 100%;
  border-top: 1px solid #ECE7E5;
  padding: 33px 0;

}
.footer_copyright .copyright{
  display: flex;
  align-items: center;
  gap: 8px;
}
.footer_copyright .media{
  display: flex;
  gap: 16px
}
</style>
