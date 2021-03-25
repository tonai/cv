<script lang="ts">
  import type { substr } from "*.gif";
  import Project from "./Project.svelte";

  export let data;
  const { projects, title } = data;
</script>

<style lang="scss">
  @import "../styles/variables";
</style>

<div class="timeline__group">
  <div class="timeline__icon" aria-hidden="true">{title.substr(0, 1)}</div>
  <h3 class="timeline__title">{title}</h3>
  <div class="timeline__content">
    {#each projects as project}
      <Project data={project} />
    {/each}
  </div>
</div>
