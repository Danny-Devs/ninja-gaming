<script>
  import Title from '$lib/title.svelte';
  import '../styles/global.css';
  const year = new Date().getFullYear();
</script>

<header>
  <Title title="Ninja Gaming Guides" />
</header>
<main>
  <!-- page content -->
  <slot></slot>
</main>
<footer>
  <p>&copy; {year} Ninja Gaming Guides</p>
</footer>

<style>
  header {
    display: flex;
    justify-content: center;
  }
  main {
    max-width: 960px;
    margin: 20px auto;
  }
  footer {
    text-align: center;
  }
</style>
