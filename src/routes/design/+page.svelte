<script>
  import { onMount } from 'svelte';
  let designContent = '';

  onMount(async () => {
    const response = await fetch('/docs/DESIGN.md');
    designContent = await response.text();
  });
</script>

<main style="border: 1px solid black; padding: 10px;">
  <h1>Design Document</h1>
  <pre>{designContent}</pre>
</main>
