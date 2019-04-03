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
  height: 60px;
  line-height: 48px;
  color: #7F8289;
  text-align: center;
}

@media (max-width: 992px) {
  .footer-wrapper {
    font-size: 14px;
  }
}
</style>
