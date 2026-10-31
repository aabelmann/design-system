<template>
  <main class="page grid">
    <header class="page__header">
      <h1>Design system</h1>
    </header>

    <AtomsSection title="Typography">
      <div class="section__rows">
        <h1>The quick brown fox jumps over the lazy dog.</h1>
        <h2>The quick brown fox jumps over the lazy dog.</h2>
        <h3>The quick brown fox jumps over the lazy dog.</h3>
        <h4>The quick brown fox jumps over the lazy dog.</h4>
        <p>The quick brown fox jumps over the lazy dog.</p>
      </div>
    </AtomsSection>
  </main>
</template>

<style lang="css" scoped>
.page__header {
  margin-bottom: var(--space-6);
}

.section__rows {
  display: flex;
  flex-direction: column;
  gap: var(--space-4);
}
</style>
