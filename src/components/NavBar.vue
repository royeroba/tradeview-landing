<script setup lang="ts">
import WorldIcon from '@/components/icons/WorldIcon.vue'
import HamburgerIcon from './icons/HamburgerIcon.vue'
import { ref } from 'vue';

const isHamburgerActivated = ref(false);
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
        <HamburgerIcon id="hamburger" @click="isHamburgerActivated = !isHamburgerActivated" />
      </div>
      <nav>
        <ul class="nav__ul disable-deco"  v-bind:style="{'display': isHamburgerActivated ? 'flex' : 'none' }">
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

<style lang="scss">
header {
  line-height: 1.5;
  display: inline;
  max-height: 10vh;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  z-index: 1;
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

#hamburger {
  display: none;
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
    width: 35%;
    margin: 0 1em;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    li {
      letter-spacing: 4px;
      color: var(--vt-c-white-mute);
      font-size: 16px;
      text-transform: uppercase;
      font-weight: bold;
    }
  }

  &__action-items {
    display: flex;
    justify-content: flex-end;
    width: 30%;
  }
}

.nav__ul {
  display: flex;
  font-size: 16px;
  align-items: center;
  width: 70%;
  padding: 2em 3em;
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

@media screen and (max-width: 1550px) {
  .header {
    background-color: var(--background-default);

    max-height: 10vh;
    &__topbar {
      flex-direction: row;
      justify-content: center;
      justify-items: center;
      align-items: center;
    }
    &__ul {
      display: none;
    }

    &__action-items {
      display: none;
    }
  }

  .logo {
    margin-left: auto;
  }
  #hamburger {
    display: block;
    width: 20px;
    margin-left: auto;
    border: 1px solid var(--vt-c-white-mute);
    padding: 16px;
    cursor: pointer;
    border-radius: 10px;
    filter: brightness(0) saturate(100%) invert(100%);
    height: auto;
    margin-right: 10%;
  }
  .nav__ul {
    flex-direction: column;
    width: 100%;
    height: 50vh;
    justify-content: center;
    align-items: center;

    background-color: var(--background-default);
    li {
      a {
        cursor: pointer;
      }
      align-items: center;
      display: flex;
      justify-content: center;
      width: 100%;
      height: 100%;

      border-bottom: 1px solid gray;
    }
    li:first-child {
      border-top: 1px solid gray;
    }
  }
}
</style>
