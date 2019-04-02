<template>
  <div id="app">
    <jl-main />
    <jl-footer />
  </div>
</template>

<script>
import JlMain from '@/components/Main'
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
/* @font-face {
  font-family: 'chicagoflfregular';
  src: url('./assets/chicagoflf-webfont.woff2') format('woff2'),
       url('/assets/chicagoflf-webfont.woff') format('woff');
  font-weight: normal;
  font-style: normal;
} */

body {
  margin: 0;
  background-color: #31333D;
}

h1 {
  margin: 0;
}

/* ------------------- Base mediaQueries and widths ------------------- */

.maxWidth {
  max-width:380px;
  margin:0 auto;
}

/* Small devices (tablets, 768px and up) */
@media (min-width:768px) {

.maxWidth {
  max-width: 100%;
  margin: 0 auto;
}

}
/* Small devices (tablets, up to 768px) */
@media (max-width:768px) {

}
/* Medium devices (desktops, between 992px and 768px) */
@media (min-width: 768px) and (max-width: 992px) {

}
/* Medium devices (desktops, up to 992px) */
@media (max-width: 992px) {

}
/*  Medium devices (desktops, 992px and up)  */
@media (min-width: 992px) {

}

/* Large devices (large desktops, 1200px and up) */
@media (min-width: 1104px) {
.maxWidth {
  max-width:1104px;
}

}
</style>
