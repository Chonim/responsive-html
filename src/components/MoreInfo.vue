<template>
  <div class="more-info-wrapper">
    <h1>Mehr Informationen</h1>
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
.more-info-wrapper {
  position: absolute;
  top: 0;
  right: 0;
  background-color: rgba(250, 250, 250, 0.8);
  width: 480px;
  height: 480px;
  padding: 32px;
  box-sizing: border-box;
  p {
    font-size: 16px;
  }
}
</style>
