<script>
  export let links = [];
</script>

<nav>
  <ul>
    {#each links as { href, label }}
      <li><a href={href}>{label}</a></li>
    {/each}
  </ul>
</nav>
