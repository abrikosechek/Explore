<template>
  <div class="main_page">
    <MPIntro />
    <TicketsPage />
    <OutroPage />
    <img src="../assets/mp_bg.png" class="mp_bg" />
  </div>
</template>

<script>
import MPIntro from "./MPIntro.vue";
import TicketsPage from "./TicketsPage.vue";
import OutroPage from "./OutroPage.vue";

export default {
  name: "MainPage",
  components: {
    MPIntro,
    TicketsPage,
    OutroPage,
  },
};
</script>

<style lang="scss">
.main_page {
  width: 100%;

  .mp_bg {
    position: absolute;
    top: 0;
    left: 0;
    z-index: -10;
    width: 100%;
    height: 750px;
  }
}
</style>
