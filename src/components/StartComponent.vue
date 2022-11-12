<template>
<div class="start__container">
  <div class="start__text-box">
    <span class="title bold">Get started now</span>
  </div>
  <div class="card__container">
    <div class="card">
      <span class="card_title bold">Connect Git repository</span>
      <span class="card_text regular">Select a Git provider to start with an existing project from any Git context.</span>
      <div class="button_wrapper">
        <div class="button gitlab">Continue with GitLab</div>
        <div class="button github">Continue with GitHub</div>
        <div class="button bitbucket">Continue with Bitbucket</div>
      </div>
      <span class="card_text regular">Or prefix any GitLab, GitHub or Bitbucket URL with <br> <p>gitpod.io/#</p></span>
    </div>
    <div class="card">

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

</style>