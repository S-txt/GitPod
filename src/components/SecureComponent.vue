<template>
<div class="secure__container">
  <span class="title bold">Remote-first. Secure by design.</span>
  <img src="../assets/code_2.png">
  <span class="text regular">
    You no longer need an over-powered laptop to code, Gitpod works just as smoothly on a Chromebook or iPad. All you need is a browser. Gitpod centralizes all source code and never stores it on insecure machines and networks.
  </span>
  <div class="extension__container">
    <div class="chrome bold">Chrome Extension</div>
    <div class="mozilla bold">Firefox Extension</div>
  </div>

</div>
</template>

<script>
export default {
  name: "SecureComponent"
}
</script>

<style scoped>
.secure__container{
  display: flex;
  flex-flow: column;
  align-items: center;
}
.title{
  font-size: 54px;
}
img{
  max-height: 820px;
  max-width: 775px;
}
.text{
  max-width: 900px;
  font-size: 24px;
  text-align: center;
}
</style>