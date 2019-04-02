<template>
  <div class="footer-wrapper">
    {{ footerText }}
  </div>
</template>

<script>
export default {
  name: 'JlFooter',
  data () {
    return {
      footerText: '© 2014 JobLeads GmbH - Alle Rechte vorbehalten'
    }
  }
}
</script>

<style lang="scss" scoped>
.footer-wrapper {
  color: #7F8289;
  text-align: center;
}
</style>
