<script>
  import Title from '$lib/title.svelte';
  import '../../styles/global.css';
  const year = new Date().getFullYear();
</script>

<header>
  <nav>
    <Title title="Ninja Gaming Guides" />
    <div class="links">
      <a href="/">Home</a>
      <a href="/about">About</a>
      <a href="/guides">Guides</a>
    </div>
  </nav>
</header>
<main>
  <!-- page content -->
  <slot />
</main>
<footer>
  <p>&copy; {year} Ninja Gaming Guides</p>
</footer>

<style>
  header {
    background: rgba(0, 0, 0, 0.2);
  }
  nav {
    max-width: 960px;
    margin: 0 auto;
    display: flex;
    align-items: center;
  }
  main {
    max-width: 960px;
    margin: 20px auto;
  }
  footer {
    text-align: center;
  }
  .links {
    margin-left: auto;
  }
  a {
    margin-left: 10px;
  }
</style>
