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
</template>

<script>

import MainComponent from "@/components/MainComponent";
import AboutComponent from "@/components/AboutComponent";
import SecureComponent from "@/components/SecureComponent";
import UsersComponent from "@/components/UsersComponent";
export default {
  name: 'App',
  components: {
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
  color: var(--black)
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
</style>
