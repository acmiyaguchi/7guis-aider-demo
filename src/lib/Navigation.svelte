<script>
  export let links = [];
</script>

<nav>
  <ul>
    <li><a href="/">Home</a></li>
    {#each links as { href, label }}
      <li><a href={href}>{label}</a></li>
    {/each}
  </ul>
</nav>
