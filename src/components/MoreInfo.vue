<template>
  <div class="more-info-wrapper">
    <img
      class="close-button"
      src="@/assets/cross.svg"
      alt="Close button"
    >
    <h1>Mehr Informationen:</h1>
    <hr>
    <p>{{ loremIpsum }}</p>
  </div>
</template>

<script>
export default {
  name: 'MoreInformation',
  data () {
    return {
      loremIpsum: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.'
    }
  }
}
</script>

<style lang="scss" scoped>
$close-button-padding: 8px;

.more-info-wrapper {
  position: absolute;
  top: 0;
  right: 0;
  background-color: rgba(250, 250, 250, 0.8);
  width: 480px;
  height: 440px;
  padding: 32px;
  box-sizing: border-box;
  .close-button {
    position: absolute;
    top: $close-button-padding;
    right: $close-button-padding;
    cursor: pointer;
  }
  h1 {
    font-size: 24px;
    font-weight: 400;
  }
  hr {
    margin-top: 28px;
    margin-bottom: 36px;
  }
  p {
    font-size: 14px;
    line-height: 1.8;
  }
}
</style>
