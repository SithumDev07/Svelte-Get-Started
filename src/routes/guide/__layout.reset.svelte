<script>
  import Logo from "$lib/logo.svelte";
</script>

<header>
  <Logo name="sithum.is/guide" />
</header>

<main>
  <!-- Main Content -->
  <slot />
</main>

<footer>
  <p>All rights reserved | 2022</p>
</footer>

<style>
  footer {
    max-width: 960px;
    margin: 3rem auto;
    font-family: "Montserrat", sans-serif;
    font-size: 2.1vw;
    color: #6160609f;
    text-align: center;
  }
</style>
