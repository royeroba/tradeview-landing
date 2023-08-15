<template>
  <div class="downloads">
    <div class="downloads__item">
      Free Download for Tradeview Users
      <button class="secondary-button">Contact your Broker</button>
    </div>
    <div class="downloads__item">
      Don’t have a Tradeview Account yet?
      <button class="primary-button">Get a Free Demo</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.downloads {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 1em;
  margin-top: 2em;
  width: 100%;
  &__item {
    display: flex;
    flex-direction: column;
    height: 100%;
    padding-right: 30px;
    margin-top: 2em;

    button {
      font-size: 18px;
      font-weight: bold;
      margin-top: 1em;
    }
  }

  &__item:not(:first-child) {
    border-left: 1px solid gray;
    padding-left: 30px;
  }

  &__item:last-child {
    border-left: 1px solid gray;
    padding-right: 0;
  }
}
</style>
