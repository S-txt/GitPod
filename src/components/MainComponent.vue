<template>
  <div class="main__container">
    <div class="main__text-box">
      <span class="main__title bold">Always<br>Ready to Code.</span>
      <span class="main__text regular">Spin up fresh, automated dev environments<br>for each task, in the cloud, in seconds.</span>
      <div class="main__button-group">
        <div class="button__wrapper">
          <div class="button bold">Try Now</div>
          <div class="icons">
            <img src="../assets/ic_gitlab.svg">
            <img src="../assets/ic_github.svg">
            <img src="../assets/ic_bitbucket.svg">
          </div>
        </div>
        <span class="regular">Open a workspace.<br>Start from any Git context.</span>
      </div>
    </div>
    <img src="../assets/room.png">
  </div>
</template>

<script>
export default {
  name: "MainComponent"
}
</script>

<style scoped>
.main__container{
  display: flex;
  flex-flow: row;
  overflow: hidden;
  padding-top: 46px;
  align-items: center;
  justify-content: space-around;
}
.main__container > img {
    max-height: 650px;
    transform: translateX(10%);
}
.main__text-box{
  display: flex;
  flex-flow: column;
  gap: 32px;
  max-width: 560px;
  transform: translateX(25%);
}
.main__title{
  font-size: 80px;
}
.main__text{
  font-size: 23px;
  color: var(--grey);
}
.button__wrapper{
  width: 160px;
  display: flex;
  flex-flow: column;
  gap: 16px;
}
.button{
  height: 46px;
  width: 160px;
  background: var(--yellow);
  line-height: 46px;
  text-align: center;
  border-radius: 16px;
}
.icons{
  display: flex;
  justify-content: space-between;
  padding: 0 8px;
}
.main__button-group{
  display: flex;
  flex-flow: row;
  gap: 24px;
}
.main__button-group span{
  color: var(--grey);
  font-size: 16px;
}

</style>