<script>
  let circles = [];
  let radius = 10;

  function addCircle(event) {
    const { offsetX, offsetY } = event;
    circles = [...circles, { x: offsetX, y: offsetY, radius }];
  }
</script>

<main style="border: 1px solid black; padding: 10px;">
  <p>This task allows drawing and manipulating circles on a canvas.</p>
  <h1>Circle Drawer</h1>
  <div>
    <label for="radius">Radius:</label>
    <input type="range" id="radius" bind:value={radius} min="1" max="100" />
  </div>
  <svg on:click={addCircle} style="border: 1px solid black; width: 100%; height: auto; max-width: 500px; max-height: 500px;">
    {#each circles as { x, y, radius }}
      <circle cx={x} cy={y} r={radius} fill="blue" />
    {/each}
  </svg>
</main>
