<template>
  <div class="navbar container">
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
  margin-top: 20px;

  .nav_logo {
    font-weight: 600;
    font-size: 36px;
    color: white;
  }

  .nav_links {
    display: flex;
    align-items: center;
    gap: 5px;

    .nav_link {
      display: block;
      height: 100%;
      padding: auto 10px;
      font-weight: 500;
      font-size: 16px;

      &:last-child {
        display: block;
        height: 100%;
        padding: auto 20px;
        background-color: #ffc814;
        font-weight: 500;
        font-size: 16px;
        color: #1f3347;
      }
    }
  }
}
</style>
