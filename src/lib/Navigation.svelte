<script>
  export let links = [];
</script>

<style>
  ul {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    padding: 0;
    list-style: none;
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
