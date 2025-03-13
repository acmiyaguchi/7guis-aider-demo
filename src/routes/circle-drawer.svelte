<script>
  let circles = [];
  let radius = 10;

  function addCircle(event) {
    const { offsetX, offsetY } = event;
    circles = [...circles, { x: offsetX, y: offsetY, radius }];
  }
</script>

<main>
  <h1>Circle Drawer</h1>
  <svg width="500" height="500" on:click={addCircle}>
    {#each circles as { x, y, radius }}
      <circle cx={x} cy={y} r={radius} fill="blue" />
    {/each}
  </svg>
</main>
