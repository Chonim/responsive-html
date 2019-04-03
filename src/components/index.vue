<template>
  <div class="jl-wrapper">
    <!-- background img -->
    <img
      class="main-background"
      src="@/assets/mood.jpg"
      alt="Mood background"
    >
    <!-- left section -->
    <section class="main-wrapper">
      <jl-logo />
      <jl-feature />
      <toggle-button
        v-show="!isMoreInfoOpen"
        @openMoreInfo="isMoreInfoOpen = true"
      />
    </section>
    <!-- right section -->
    <section>
      <more-info
        v-show="isMoreInfoOpen"
        @closeMoreInfo="isMoreInfoOpen = false"
      />
    </section>
  </div>
</template>

<script>
import JlLogo from '@/components/Header/Logo'
import JlFeature from '@/components/Main/Feature'
import ToggleButton from '@/components/Main/ToggleButton'
import MoreInfo from '@/components/Main/MoreInfo'

export default {
  name: 'JlMain',
  components: {
    JlLogo,
    JlFeature,
    ToggleButton,
    MoreInfo
  },
  data () {
    return {
      isMoreInfoOpen: false
    }
  }
}
</script>

<style lang="scss" scoped>
.jl-wrapper {
  position: relative;
  margin: 0 auto;
  display: flex;
  width: 992px;
  .main-background {
    flex: 1;
    height: calc(100vh - 60px);
    max-width: 992px;
  }
  .main-wrapper {
    position: absolute;
    top: 40px;
    left: 40px;
    width: 440px;
    height: auto;
    margin: 0 auto;
  }
}

@media (max-width: 992px) {
  .jl-wrapper {
    width: 100%;
    display: block;
    .main-background {
      display: none;
    }
    .main-wrapper {
      position: relative;
      top: 0;
      left: 0;
      width: 100vw;
      margin: 0 auto;
    }
  }
}
</style>
