<template>
<users__container>
  <users__text-box>
    <span class="title bold">
      Used by 400,000+ developers.
    </span>
  </users__text-box>
  <div class="cards__container">
    <card-component
        text="GitPod is incredibly cool. \n \n In my opinion, this is a big step in open source software contribution. I'm excited to see where we go from here."
        img='../assets/ic_user.svg'
        name="Ben Halpern"
        position="Creator and Co-founder <b>@forem<b/> and <b>@ThePracticalDev<b/>"
    />
  </div>
</users__container>
</template>

<script>
import CardComponent from "@/components/CardComponent";
export default {
  name: "UsersComponent",
  components: {CardComponent}
}
</script>

<style scoped>

</style>