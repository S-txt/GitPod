<template>
<div class="about__container">
  <div class="about__text-group">
    <div class="about__text-box">
    <span class="title bold">
      Think CI/CD for dev environments
    </span>
      <span class="text regular">
      We invented prebuilds so application code, configuration and infrastructure can all be stored as machine-executable code in your git repositories and applied to dev environments automatically and continuously.</span>
    </div>
    <div class="about__button-container">
      <div class="button bold">More on prebuilds</div>
      <div class="button bold">Documentation</div>
    </div>
  </div>
  <img src="../assets/code_1.png">
</div>
</template>

<script>
export default {
  name: "AboutComponent"
}
</script>

<style scoped>

.about__container{
  display: flex;
  flex-flow: row;
  margin: 200px 20px;
  justify-content: space-around;
  align-items: center;
  max-height: 470px;
  height:470px
}
.about__container img{
  max-height: 470px;
}
.about__text-box{
  display: flex;
  flex-flow: column;
  gap: 8px;
  max-width: 655px;
}
.about__text-box .bold{
  font-size: 32px;
}
.about__text-box .regular{
  font-size: 24px;
  color: var(--grey);
}


.about__text-group{
  display: flex;
  height: 100%;
  flex-flow: column;
  justify-content: space-between;
}

.about__button-container{
  display: flex;
  flex-flow: row;
  gap: 16px;
  transform: translateY(-15%);
}
.button{
  padding: 7px 18px;
  border-radius: 10px;
  font-size: 14px;
}
.about__button-container .button:nth-child(1){
  background-color: var(--yellow);
}
.about__button-container .button:nth-child(2) {
  background-color: var(--pink);
 }

</style>