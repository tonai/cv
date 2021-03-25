<style lang="scss">
  @import "../styles/variables";

  :root {
    --bg-color: #{$bgColor};
    --font-color: #{$fontColor};
    --primary-color: #{$primaryColor};
  }

  :global(body) {
    background: var(--bg-color);
    color: var(--font-color);
  }

  .Layout {
    display: grid;
    grid-template-columns: auto 1fr;
    grid-template-rows: auto;
    grid-gap: 0;
    grid-template-areas:
      "colHeader main"
      "col main";
  }

  .Layout__colHeader {
    padding-left: $padding;
    padding-right: $padding;
    grid-area: colHeader;
  }

  .Layout__main {
    padding-left: $padding;
    padding-right: $padding;
    grid-area: main;
  }

  .Layout__col {
    padding-left: $padding;
    padding-right: $padding;
    grid-area: col;
  }
</style>

<div class="Layout">
  <div class="Layout__colHeader">
    <slot name="colHeader" />
  </div>
  <main class="Layout__main">
    <slot name="main" />
  </main>
  <div class="Layout__col">
    <slot name="col" />
  </div>
</div>
