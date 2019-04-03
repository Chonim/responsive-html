<template>
  <div id="app">
    <jl-main />
    <jl-footer />
  </div>
</template>

<script>
import JlMain from '@/components'
import JlFooter from '@/components/Footer'

export default {
  name: 'app',
  components: {
    JlMain,
    JlFooter
  }
}
</script>

<style lang="scss">
body {
  font-family: 'Fira Sans';
  margin: 0;
  background-color: #31333D;
}

h1 {
  margin: 0;
}
</style>
