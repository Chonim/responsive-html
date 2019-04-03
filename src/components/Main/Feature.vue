<template>
  <div class="feature-wrapper">
    <div class="feature-title">
      <div>{{ featureTitle }}</div>
      <img
        class="feature-image"
        src="@/assets/mood-mobile.jpg"
        alt="Feature Image"
      >
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
  min-height: 340px;
  height: auto;
  background-color: #fff;
  margin-top: 40px;
  .feature-title {
    font-size: 22px;
    padding: 16px;
    box-sizing: border-box;
    line-height: 1.4;
    color: #F9FBFF;
    background-color: #31333D;
    .feature-image {
      display: none;
    }
  }
  .feature-list-container {
    margin-top: 32px;
    .feature-list {
      padding-left: 16px;
      font-size: 14px;
      font-weight: 400;
      li {
        display: flex;
        align-items: baseline;
        line-height: 2;
        img {
          margin-right: 10px;
        }
      }
    }
  }
  .price-wrapper {
    display: flex;
    align-items: flex-end;
    width: 240px;
    margin: 0 auto;
    margin-top: 36px;
    .check-mark-circle {
      margin-right: 20px;
    }
    .discounted-price {
      color: #31333D;
      font-size: 32px;
      font-weight: 500;
    }
    .original-price {
      font-size: 12px;
      text-decoration-line: line-through;
    }
  }
}

@media (max-width: 992px) {
  .feature-wrapper {
    margin-top: 0px;
    .feature-title {
      font-size: 16px;
      line-height: 1.6;
      .feature-image {
        display: block;
        height: 172px;
        width: auto;
        margin: 16px auto 4px;
      }
    }
    .feature-list-container {
      width: 288px;
      margin: 0 auto;
      .feature-list {
        font-size: 12px;
        li {
          line-height: 2;
        }
      }
    }
    .price-wrapper {
      padding-bottom: 32px;
    }
  }
}
</style>
