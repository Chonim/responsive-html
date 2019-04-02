<template>
  <div class="logo-wrapper">
    <img
      src="@/assets/logo_JL.svg"
      alt="Job Leads Logo"
    >
  </div>
</template>

<script>
export default {
  name: 'JlLogo'
}
</script>

<style lang="scss" scoped>
.logo-wrapper {
  background-color: #fff;
  position: absolute;
  top: 40px;
  left: 40px;
  /* width: 280px;
  height: 80px; */
  display: flex;
  img {
    flex: 1;
    padding: 12px;
    box-sizing: border-box;
  }
}
</style>
