<script context="module">
  export async function load() {
    const response = await import('./DESIGN.svx');
    return {
      designContent: response.default
    };
  }
</script>

<main style="border: 1px solid black; padding: 10px;">
  <h1>Design Document</h1>
  <article>
    {@html designContent}
  </article>
</main>
