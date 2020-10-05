<template>
  <div class="about-me">
    <div class="picture-container">
      <img />
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
  display: flex;
  flex-direction: column;
  align-items: center;
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 38.2%;
  background: $-sliver;
  background-image: linear-gradient($-gray, $-sliver);
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
}
.line {
  margin-top: $-fib-px * 2;
  margin-bottom: $-fib-px * 4;
  width: $-fib * 2;
  height: $-fib-px / 2;
  background: $-aqua;
  opacity: 0.2;
}
</style>
