<template>
  <section class="section">
    <div class="section__header">
      <h2 id="font-sizes">{{ title }}</h2>
    </div>
    <div class="section__content">
      <slot></slot>
    </div>
  </section>
</template>

<script setup lang="ts">
defineProps<{
  title: string;
}>();
</script>


<style lang="css" scoped>
.section {
  display: grid;
  grid-template-rows: min-content 1fr;
  gap: var(--space-4);
}

.section__header {
  grid-row: 1;
}

.section__content {
  grid-row: 2;
}
</style>
