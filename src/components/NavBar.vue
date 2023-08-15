<script setup lang="ts">
import WorldIcon from '@/components/icons/WorldIcon.vue'
</script>

<template>
  <header>
    <div>
    <div class="header__topbar">
      <img alt="Tradeview logo" class="logo" src="@/assets/logo.svg" />

      <ul class="header__ul disable-deco">
        <li>Forex</li>
        <li>Stock</li>
        <li>Futures</li>
        <li>TradeGATEHub</li>
      </ul>

      <div class="header__action-items">
        <p class="filled-arrow-down clickable">Log In</p>
        <span class="separator" />
        <p class="clickable">Contact Us</p>
        <p class="clickable">English <WorldIcon /></p>
      </div>
    </div>

    <nav>
      <ul class="nav__ul disable-deco">
        <li>
          <a href="/">Markets</a>
        </li>
        <li>
          <a href="/" class="filled-arrow-down">Company</a>
        </li>
        <li>
          <a href="/">Accounts</a>
        </li>
        <li>
          <a href="/">Platforms</a>
        </li>
        <li>
          <a href="/">Pricing</a>
        </li>
        <li>
          <a href="/">Introducing Brokers</a>
        </li>
        <li>
          <a href="/">Education</a>
        </li>
        <li>
          <a href="/">Support</a>
        </li>
      </ul>
    </nav>
  </div>
  </header>
</template>

<style scoped lang="scss">
header {
  line-height: 1.5;
  display: inline;
  max-height: 10vh;
  position: -webkit-sticky;
  position: sticky;
  top: 0;

}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  background: transparent
    linear-gradient(180deg, #181f29 0%, #181f29 18%, #181f2960 59%, #181f2900 100%) 0% 0% no-repeat
    padding-box;

  li a {
    color: var(--vt-c-white-mute);
  }
}

.logo {
  width: 365;
  height: 55;
  margin: 0;
  padding: 0;
}

.header {
  background-color: var(--background-default);
  &__topbar {
    background-color: var(--background-default);
    display: flex;
    align-items: center;
    padding: 0.5em 0;
    justify-content: space-around;
  }

  &__ul {
    display: flex;
    width: 30%;
    margin: 0 1em;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    li {
      color: var(--vt-c-white-mute);
      font-size: 16px;
      text-transform: uppercase;
      font-weight: bold;
    }
  }

  &__action-items {
    display: flex;
    justify-content: flex-end;
    width: 40%;
  }
}

.nav__ul {
  display: flex;
  font-size: 16px;
  align-items: center;
  width: 70%;
  padding: 1em 3em;
  justify-content: space-between;

  li {
    a {
      @extend .disable-deco !optional;
      list-style-type: none;
      pointer-events: none;
      text-decoration: none;
    }
  }
}
</style>
