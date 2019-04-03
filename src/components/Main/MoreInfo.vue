<template>
  <div class="more-info-wrapper">
    <img
      class="close-button"
      src="@/assets/cross.svg"
      alt="Close button"
      @click="$emit('closeMoreInfo')"
    >
    <h1>Mehr Informationen:</h1>
    <hr>
    <p>{{ loremIpsum }}</p>
  </div>
</template>

<script>
import loremIpsum from './lorem-ipsum'

export default {
  name: 'MoreInformation',
  data () {
    return {
      loremIpsum
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
  width: 440px;
  min-height: 360px;
  padding: 24px 20px;
  box-sizing: border-box;
  .close-button {
    position: absolute;
    top: $close-button-padding;
    right: $close-button-padding;
    cursor: pointer;
  }
  h1 {
    font-size: 20px;
    font-weight: 300;
  }
  hr {
    margin-top: 28px;
    margin-bottom: 36px;
  }
  p {
    font-size: 12px;
    font-weight: 300;
    line-height: 1.8;
  }
}

@media (max-width: 992px) {
  .more-info-wrapper {
    position: relative;
    width: 100vw;
    background-color: #fff;
  }
}
</style>
