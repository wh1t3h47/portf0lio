<template>
  <topBar />
  <aboutMe />
  <textFeed />
</template>

<script>
import textFeed from "./components/feed";
import aboutMe from "./components/sideAboutMe"
import topBar from "./components/topBar"

export default {
  name: "App",
  components: {
    aboutMe,
    textFeed,
    topBar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
