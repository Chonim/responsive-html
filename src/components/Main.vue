<template>
  <div class="jl-wrapper">
    <!-- background img -->
    <img
      class="main-background"
      src="@/assets/mood.jpg"
      alt="Mood background"
    >
    <section class="main-wrapper">
      <!-- header -->
      <jl-logo />
      <!-- main -->
      <jl-feature />
    </section>
    <more-info />
  </div>
</template>

<script>
import JlLogo from '@/components/Header/Logo'
import JlFeature from '@/components/Main/Feature'
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
.jl-wrapper {
  position: relative;
  margin: 0 auto;
  display: flex;
  width: 90%;
  .main-background {
    flex: 1;
    height: calc(100vh - 60px);
  }
  .main-wrapper {
    position: absolute;
    top: 40px;
    left: 40px;
    width: 460px;
    margin: 0 auto;
  }
}
</style>
