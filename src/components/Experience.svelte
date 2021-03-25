<script lang="ts">
  import Company from "./Company.svelte";
  import smile from "../data/smile.json";
</script>

<div class="block">
  <h2 class="block__title">Expérience</h2>
  <div class="timeline">
    <Company data={smile} />
    <Company data={smile} />
  </div>
</div>
