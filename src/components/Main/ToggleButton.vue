<template>
  <transition name="fade">
    <button
      class="more-info-button"
      @click="$emit('openMoreInfo')"
    >
      Jetzt säubern und neuen job finden
    </button>
  </transition>
</template>

<script>
export default {
  name: 'ToggleButton'
}
</script>

<style lang="scss" scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity .3s ease;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}

.more-info-button {
  width: 100%;
  height: 52px;
  color: #fff;
  font-size: 16px;
  background-color: #FF7503;
  border: none;
  transition: 0.2s;
  font-weight: 600;
  cursor: pointer;
  &:hover {
    font-size: 18px;
  }
}

@media (max-width: 992px) {
 .more-info-button {
   font-size: 1.6vw;
 }
}

@media (max-width: 768px) {
  .more-info-button {
   font-size: 12px;
 }
}
</style>
