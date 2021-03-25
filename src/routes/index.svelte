<script lang="ts">
  import Contact from "../components/Contact.svelte";
  import Experience from "../components/Experience.svelte";
  import Interests from "../components/Interests.svelte";
  import Introduction from "../components/Introduction.svelte";
  import Language from "../components/Language.svelte";
  import Layout from "../components/Layout.svelte";
  import Education from "../components/Education.svelte";
  import Profile from "../components/Profile.svelte";
  import Skills from "../components/Skills.svelte";
</script>

<style global lang="scss">
  @import "../styles/main";
</style>

<svelte:head>
  <title>Curriculum Vitæ Tony Cabaye</title>
  <meta
    name="description"
    content="Expert Technique et tech lead full stack JavaScript avec spécialité Frontend sur les technologies React et Angular" />
</svelte:head>

<Layout>
  <div slot="colHeader">
    <Profile />
  </div>
  <div slot="main">
    <Introduction />
    <Experience />
    <Education />
  </div>
  <div slot="col">
    <Contact />
    <Skills />
    <Language />
    <Interests />
  </div>
</Layout>
