<script>
  export let links = [];
</script>

<style>
  nav {
    padding: 10px;
  }
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    gap: 10px;
  }
  a {
    text-decoration: none;
    color: black;
  }
</style>

<nav>
  <ul>
    <li><a href="/">Home</a></li>
    {#each links as { href, label }}
      <li><a href={href}>{label}</a></li>
    {/each}
  </ul>
</nav>
