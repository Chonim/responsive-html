<template>
  <div class="feature-wrapper">
    <div class="feature-title">
      {{ featureTitle }}
    </div>
    <div class="feature-list-container">
      <ul class="feature-list">
        <li
          v-for="feature in features"
          :key="feature"
        >
          <img src="@/assets/arrow.svg" alt="Check mark">
          <div>{{ feature }}</div>
        </li>
      </ul>
      <div class="price-wrapper">
        <img
          class="check-mark-circle"
          src="@/assets/arrowCircle.svg"
          alt="Check mark"
        >
        <div>
          <div class="discounted-price">EUR 79.40</div>
          <div class="original-price">EUR 13,23 pro Monat</div>
        </div>
      </div>
    </div>
    <!-- <button class="more-info-button">
      Jetzt säubern und neuen job finden
    </button> -->
  </div>
</template>

<script>
export default {
  name: 'JlFeature',
  data () {
    return {
      featureTitle: 'Sehr geehrter Herr Mustermann, starten Sie sauber ins jahr 2015 mit neuen Perspektiven.',
      features: [
        'Unbegrenzte Ansicht aller Premiun-jobs',
        'Gezielte Filtermöglichkeiten nach jobs mit mehr Gehalt'
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.feature-wrapper {
  width: 100%;
  height: 360px;
  background-color: #fff;
  margin-top: 40px;
  .feature-title {
    font-size: 22px;
    padding: 16px;
    box-sizing: border-box;
    line-height: 1.4;
    color: #F9FBFF;
    background-color: #31333D;
  }
  .feature-list-container {
    margin-top: 32px;
    .feature-list {
      padding-left: 16px;
      font-size: 16px;
      li {
        display: flex;
        line-height: 1.6;
        img {
          margin-right: 10px;
        }
      }
    }
  }
  .price-wrapper {
    display: flex;
    width: 76%;
    margin: 0 auto;
    margin-top: 36px;
    .check-mark-circle {
      margin-right: 20px;
    }
    .discounted-price {
      font-size: 40px;
    }
    .original-price {
      text-decoration-line: line-through;
    }
  }
  .more-info-button {
    width: 100%;
    height: 52px;
    color: #fff;
    font-size: 18px;
    background-color: #FF7503;
    border: none;
    transition: 0.2s;
    &:hover {
      font-size: 20px;
    }
  }
}
</style>
