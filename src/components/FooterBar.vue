<script setup lang="ts">
import TermsText from '@/components/TermsText.vue'
</script>

<template>
  <footer>
    <div class="footer__information">
      <div>
        <img alt="Tradeview logo" class="logo" src="@/assets/logo.svg" width="40%" />
        <p>
          <strong> Tradeview Markets </strong>| Grand Cayman, KY1-1002, 4th Floor Harbour Place |
          103 South Church St, PO Box 1105
        </p>
        <p>
          <strong> Main Oﬃce: </strong>
          +1 345 945 6271
        </p>
        <p>
          <strong> Direct Phone: </strong>
          +1 345 946 4532
        </p>
        <p>
          <strong> Website: </strong>
          www.tvmarkets.com
        </p>
      </div>
      <div id="newsletter">
        <div id="newsletter__title">
          <img alt="Tradeview logo" class="logo" src="@/assets/logo.svg" />
          <p>
            Find daily trading insights and understand what is behind the latest waves in financial
            markets.
          </p>
        </div>
        <div id="newsletter__form">
          <input placeholder="Enter your email address" />
          <button class="secondary-button">Subscribe</button>
        </div>
      </div>
    </div>
    <TermsText />
  </footer>
</template>

<style lang="scss" scoped>
footer {
  color: var(--vt-c-white-mute);
  padding: 5% 10%;
  padding-bottom: 10%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-top: auto;

  background-color: var(--background-footer);
  img {
    filter: brightness(0) saturate(100%) invert(100%);
  }
  &strong {
    font-weight: bold;
  }
}

strong{
        font-weight: bold;
    }

.footer {

  &__information {
    display: flex;
    justify-content: space-between;
    margin-top: auto;
    flex-direction: row;
    gap: 6em;
  }
}

#newsletter {
  display: flex;
  flex-direction: column;
  gap: 2em;
  border: 1px solid var(--text-color-terms);
  padding: 2em 5em;

  &__title {
    display: flex;
    gap: 3em;
    justify-content: center;
    img {
      width: 220px;
      padding-right: 3em;
      border-right: 1px solid var(--text-color-terms);
    }

    p {
      font-weight: bold;
    }

  }

  &__form{

    display: flex;
    gap: 3em;
        justify-content: space-between;
    input{
        all: unset;
        border: 1px solid var(--text-color-terms);
        padding: 1em;
        justify-content: center;
        flex:4

    }

    button {
        flex: 1.5;
        background-color: var(text-color);
    }
  }

}
</style>
