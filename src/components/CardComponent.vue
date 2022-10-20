<template>
  <div class="card">
    <span class="card__text">{{text}}</span>
    <div class="card__user">
      <img class="user__img" src="{{img}}">
      <span class="user__name bold">{{name}}</span>
      <span class="user__position">{{position}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props:{
    'text': String,
    'img': URL,
    'name': String,
    'position': HTMLAllCollection

  }
}
</script>

<style scoped>
  .card{
    display: flex;
    flex-flow: column;

    font-size: 16px;
    width: calc(384px - 48px);
    gap:16px;
    padding: 24px;
    background: white;
    border-radius: 16px;
  }
  .card__user{
    display: flex;
    flex-flow: row;
    gap: 12px;
  }
  .user__img{
    height: 48px;
    width: 48px;
    border-radius: 50%;
  }

</style>