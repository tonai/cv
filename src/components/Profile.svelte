<script lang="ts">
  import profile from "images/tony.jpg";
</script>

<style lang="scss">
  @import "../styles/variables";

  .Profile {
    width: 200px;
    border-radius: 50%;
    filter: grayscale(100%);
  }
</style>

<div class="block"><img alt="Tony Cabaye" class="Profile" src={profile} /></div>
