<script setup lang="ts">
defineProps(['title', 'description'])
</script>

<template>
  <aside class="card">
    <slot class="icon"></slot>
    <h4 class="card__title">{{ title }}</h4>
    <p class="card__description">{{ description }}</p>
  </aside>
</template>

<style lang="scss">
.card {
  padding: 1em;
  display: flex;
  flex-direction: column;
  padding: 2em;
  gap: 0.5em;
  justify-content: flex-start;
  background-color: #ffffff 0% 0% no-repeat padding-box;
  box-shadow: 0px 0px 30px #00000014;
  color: var(--text-color);

  &__title{
    font-size: 18px;
    color:red;
    font-weight: bold;
  }
}

.description {
  flex: 1;
  margin-left: 1rem;
}

.icon {
}
</style>
