<template>
  <div class="intro">
    <h1>It is a Big World Out There, Go Explore</h1>
    <p>
      Conveniently customize proactive web services for leveraged without continualliery
      aggregate fricctionle ou wellies richard.and very customize continually.
    </p>
    <div class="links_group">
      <router-link to="/main">Get exploration</router-link>
      <router-link to="/main">Read more</router-link>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.intro {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 1320px;
  margin: 110px auto;
  gap: 30px;

  & > h1 {
    max-width: 570px;
    font-weight: 700;
    font-size: 64px;
    line-height: 1em;
    color: white;
  }
  & > p {
    max-width: 570px;
    font-weight: 400;
    font-size: 16px;
    line-height: 2em;
    color: white;
  }

  .links_group {
    display: flex;
    gap: 15px;

    & > a:first-child {
      padding: 12px 16px;
      background-color: #ffc814;
      border-radius: 4px;
      font-weight: 500px;
      font-size: 16px;
    }

    & > a:last-child {
      padding: 12px 16px;
      background-color: #fffdfd;
      border-radius: 4px;
      font-weight: 500px;
      font-size: 16px;
    }
  }
}
</style>
