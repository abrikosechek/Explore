<template>
  <div class="navbar">
    <router-link to="/main" class="nav_logo">Explore</router-link>
    <div class="nav_links">
      <router-link to="/main" class="nav_link">home</router-link>
      <router-link to="/main" class="nav_link">tours</router-link>
      <router-link to="/main" class="nav_link">hotel</router-link>
      <router-link to="/main" class="nav_link">gallery</router-link>
      <router-link to="/main" class="nav_link">pages</router-link>
      <router-link to="/main" class="nav_link">blog</router-link>
      <router-link to="/main" class="nav_link">contact</router-link>
      <router-link to="/main" class="nav_link">login</router-link>
      <router-link to="/main" class="nav_link">Sign UP</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavigBar",
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  max-width: 1320px;
  margin: 15px auto 0;

  .nav_logo {
    font-weight: 600;
    font-size: 36px;
    color: white;
  }

  .nav_links {
    display: flex;
    align-items: center;
    gap: 30px;

    .nav_link {
      font-weight: 500;
      font-size: 18px;
      text-transform: capitalize;
      color: white;

      &:last-child {
        padding: 12px 26px;
        background-color: #ffc814;
        border-radius: 4px;
        font-weight: 600;
        font-size: 14px;
        color: #1f3347;
      }
    }
  }
}
</style>
