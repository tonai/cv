<script lang="ts">
  export let data;
  const { end, title } = data;
  const now = new Date();
</script>

<style lang="scss">
  @import "../styles/variables";
</style>

<div class="Project timeline__subGroup">
  <h4 class="timeline__subTitle">{title}</h4>
  <h4 class="timeline__end">
    <span class="visually-hidden">Terminée le
    </span>{end === 'now' ? `${String(now.getMonth() + 1).padStart(2, '0')}/${now.getFullYear() + 1}` : end}
  </h4>
  <p class="timeline__subContent">...</p>
</div>
