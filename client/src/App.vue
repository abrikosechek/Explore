<template>
  <NavigBar />
  <router-view />
</template>

<script>
import NavigBar from "./components/NavigBar.vue";

export default {
  name: "App",
  components: {
    NavigBar,
  },
};
</script>

<style lang="scss">
$dark-blue: #1f3347;
$warning: #ffc814;

#app {
  font-family: "Poppins", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  margin: 0;
}

* {
  box-sizing: border-box;
}

h1,
h2,
h3,
h4,
h5,
h6,
p,
a,
span,
label {
  margin: 0;
  padding: 0;
}

button {
  background-color: $warning;

  & > * {
    color: #1f3347;
  }
  cursor: pointer;
}

.container {
  max-width: 1320px;
  margin: 0 auto;
}

@media (max-width: 1360px) {
  .container {
    width: 100%;
    margin: 0 20px;
  }
}
</style>
