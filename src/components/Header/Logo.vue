<template>
  <header class="logo-wrapper">
    <img
      src="@/assets/logo_JL.svg"
      alt="Job Leads Logo"
    >
  </header>
</template>

<script>
export default {
  name: 'JlLogo'
}
</script>

<style lang="scss" scoped>
.logo-wrapper {
  background-color: #fff;
  width: 320px;
  display: flex;
  img {
    flex: 1;
    padding: 12px;
    box-sizing: border-box;
  }
}

@media (max-width: 992px) {
  .logo-wrapper {
    width: 100%;
    padding-top: 8px;
  }
}
</style>
