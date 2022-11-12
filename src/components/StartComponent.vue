<template>
<div class="start__container">
  <div class="start__text-box">
    <span class="title bold">Get started now</span>
  </div>
  <div class="card__container">
    <div class="card_git">
      <div class="card_content">
        <span class="card_title bold">Connect Git repository</span>
        <span class="card_text regular">Select a Git provider to start with an existing project from any Git context.</span>
      </div>
      <div class="button_wrapper">
        <div class="button gitlab">
          <img src="../assets/ic_gitlab_white.svg">
          Continue with GitLab</div>
        <div class="button github">
          <img src="../assets/ic_github_white.svg">
          Continue with GitHub</div>
        <div class="button bitbucket">
          <img src="../assets/ic_bitbucket_white.svg">
          Continue with Bitbucket</div>
      </div>
      <span class="card_text regular">Or prefix any GitLab, GitHub or Bitbucket URL with <br> <div class="tag">gitpod.io/#</div></span>
    </div>
    <div class="card_launch">
      <div class="card_content">
        <span class="card_title bold"> Launch an example workspace</span>
        <span class="card_text regular">Dive into one of our example workspaces</span>
      </div>
      <div class="button_wrapper regular">
        <div class="button typescript">
          <div>
          <img src="../assets/ic_typescript.svg">
          <span>Node or TypeScript</span>
          </div>
          <div class="launch">Launch workspace</div>
        </div>
        <div class="button python">
          <div>
          <img src="../assets/ic_python.svg">
          <span>Python</span>
          </div>
          <div class="launch">Launch workspace</div>
        </div>
        <div class="button go">
          <div>
          <img src="../assets/ic_go.svg">
          <span>Go</span>
          </div>
          <div class="launch">Launch workspace</div>

        </div>
        <div class="button rust">
          <div>
          <img src="../assets/ic_rust.svg">
          <span>Rust</span>
          </div>
          <div class="launch">Launch workspace</div>
        </div>
        <div class="button java">
          <div>
          <img src="../assets/ic_java.svg">
          <span>Java</span>
          </div>
          <div class="launch">Launch workspace</div>
        </div>
        <div class="button svelte">
          <div>
          <img src="../assets/ic_svelte.svg">
          <span>Svelte</span>
          </div>
          <div class="launch">Launch workspace</div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: "StartComponent"
}
</script>

<style scoped>
.start__container{
  display: flex;
  flex-flow: column;
  align-items: center;
  margin: 212px 0;
  gap: 48px
}
.title{
  font-size: 54px;
}
.card__container{
  display: flex;
  flex-flow: row;
  justify-content: center;
  gap: 26px;
  flex-wrap: wrap;
}
.card_git, .card_launch{
  display: flex;
  flex-flow: column;
  background-color: #FFFFFF;
  color: var(--black);
  border-radius: 20px;
  padding: 56px 56px 56px 86px;
  width: 642px;
  text-align: center;
  gap: 64px;
}
.card_content{
  display: flex;
  flex-flow: column;
}
.card_title{
  font-size: 32px;
}
.card_text{
  font-size: 24px;
  display: flex;
  flex-flow: column;
  align-items: center;
}
.tag{
  display: flex;
  background-color: var(--peach);
  border-radius: 12px;
  max-width: 151px;
  justify-content: center;
  padding: 0 16px;
}
.button_wrapper{
  display: flex;
  flex-flow: column;
  align-self: center;
  gap:16px;
}
.button{
  display: flex;
  height: 56px;
  border-radius: 12px;
  background-color: #2684FF;
  align-items: center;
  gap: 16px;
  width: 262px;
  padding-left: 33px;
}
.button_wrapper .gitlab{
  background:var(--orange);
  color: #FFFFFF;
}
.button_wrapper .github{
  background-color: black;
  color: #FFFFFF;
}
.button_wrapper .bitbucket{
  background-color: var(--blue);
  color: #FFFFFF;
}
.card_launch .button_wrapper .button{
  display: flex;
  background-color: #F9F9F9;
  width: 506px;
  justify-content: space-between;
  align-items: center;
  padding: 12px;
}
.button:hover{
  cursor: pointer;
}
.card_launch .button_wrapper .button > div{
  display: flex;
  gap: 16px
}
.card_launch .button_wrapper .button .launch{
  background-color: var(--black);
  color: #FFFFFF;
  border-radius: 12px;
  padding: 7px 12px;
  transition: linear 0.3s;
}
.card_launch .button_wrapper .button .launch:hover{
  background-color: var(--grey);


}
</style>