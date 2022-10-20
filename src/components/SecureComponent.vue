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
  gap: 48px
}
.title{
  font-size: 54px;
}
img{
  width: 820px;
  max-width: 820px;
  box-shadow: -2px 2px 15px 8px var(--yellow);
  border-radius: 14px;
}
.text{
  max-width: 900px;
  font-size: 24px;
  text-align: center;
  color: var(--grey);
}
.extension__container{
  display: flex;
  flex-flow: row;
  gap:16px
}
.extension__container .bold{
  padding: 8px 12px 8px 46px;
  font-size: 18px;
}
.chrome{
  background: url("../assets/ic_mozilla.svg") 7% center no-repeat, white;
}
.mozilla{
  background: url("../assets/ic_mozilla.svg") 7% center no-repeat, white;
}
</style>