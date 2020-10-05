<template>
  <div class="about-me">
    <div class="picture-container">
      <img src="@/assets/logo.png" />
    </div>
    <div class="line"></div>
    <div class="information-container"></div>
  </div>
</template>

<script>
export default {
  name: "aboutMe",
};
</script>

<style scoped lang="scss">
@import "./index.scss";
.about-me {
  @include gradient-alpha-bg(to top, 1, $-urban-day, $-urban);
  border-radius: 0 $-fib-px;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 38.2%;
  &:hover {
    box-shadow: $-fib-px 0 $-fib-px * 2 $-sliver-aura;
  }
}
.picture-container {
  margin-top: $-fib-px * 10;
  height: $-fib-px * 50;
  width: $-fib-px * 50;
  border-radius: 50%;
  background: $-olive;
  img {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
    border-radius: inherit;
  }
}
.line {
  align-self: center;
  border-radius: $-fib-px;
  margin-top: $-fib-big-px;
  /** the bottom container is 2 times bigger than top
   *  so I keep margin-bottom 2 times bigger as well
   */
  margin-bottom: $-fib-big-px * 2;
  width: 100% - $-fib;
  height: $-fib-px;
  background: $-before-morning;
  opacity: 0.2;
}
.information-container {
  background: radial-gradient($-foggy-morning, $-night-blue);
  border-radius: $-fib-px * 10;
  opacity: $-fib-mul * 3;
  height: 50%;
  width: $-fib * 2;
}
</style>
