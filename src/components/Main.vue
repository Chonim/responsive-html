<template>
  <div class="main-wrapper">
    <img
      class="main-background"
      src="@/assets/mood.jpg"
      alt="Mood background"
    >
    <jl-logo />
    <jl-feature />
    <more-info />
  </div>
</template>

<script>
import JlLogo from '@/components/Logo'
import JlFeature from '@/components/Feature'
import MoreInfo from '@/components/MoreInfo'

export default {
  name: 'JlMain',
  components: {
    JlLogo,
    JlFeature,
    MoreInfo
  }
}
</script>

<style lang="scss" scoped>
.main-wrapper {
  position: relative;
  width: 90%;
  margin: 0 auto;
  display: flex;
  .main-background {
    flex: 1;
    height: 100vh;
  }
}
</style>
